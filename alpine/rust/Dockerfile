FROM alpine:edge

RUN apk update && apk add musl-dev gcc libgcc llvm clang lld lldb

ENV RUSTUP_HOME=/usr/local/rustup \
    CARGO_HOME=/usr/local/cargo \
    PATH=/usr/local/cargo/bin:$PATH

RUN rust_arch=x86_64-unknown-linux-musl \
    url="https://static.rust-lang.org/rustup/dist/${rust_arch}/rustup-init"; \
    wget $url; \
    chmod +x rustup-init; \
    ./rustup-init -y --no-modify-path --default-toolchain nightly; \
    rm rustup-init; \
    chmod -R a+w $RUSTUP_HOME $CARGO_HOME; \
    rustup --version; \
    cargo --version; \
    rustc --version;
RUN rustup component add rust-src rustc-dev llvm-tools-preview
