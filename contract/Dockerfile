# Base image
FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

# Install system dependencies (build-essential, CMake, Rust, Git, etc.)
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    wget \
    git \
    cmake \
    ninja-build \
    zlib1g-dev \
    libsecp256k1-dev \
    libmicrohttpd-dev \
    libsodium-dev \
    pkg-config \
    openssl \
    libssl-dev \
    python3 \
    python3-pip \
    unzip \
    sudo \
    vim \
    && rm -rf /var/lib/apt/lists/*

# Install Rust for tonos-cli
RUN curl https://sh.rustup.rs -sSf | bash -s -- -y
ENV PATH="/root/.cargo/bin:${PATH}"

# Set working directory
WORKDIR /app

# Copy contract repo into the image
COPY . .

# Build tonos-cli from local source
RUN cd tonos-cli && cargo build --release && cp target/release/ever-cli /usr/local/bin/tonos-cli

# Build TON core tools from source (FunC, Fift, lite-client)
RUN mkdir -p ton/build && cd ton/build \
    && cmake .. -DCMAKE_BUILD_TYPE=Release \
    && make -j$(nproc) \
    && find ./ -type f -perm /111 -exec cp {} /usr/local/bin/ \;

# Set working directory where contract lives
WORKDIR /app/contract

# Add entrypoint for dev/testing
CMD ["/bin/bash"]
