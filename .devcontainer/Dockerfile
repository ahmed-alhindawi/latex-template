FROM docker.io/alpine:3.21

# Install required packages
RUN apk update && apk add --no-cache \
    git \
    texlive-full \
    openssh \
    && rm -rf /var/cache/apk/*

# # Install cpanminus and required Perl modules for latexindent
# RUN curl -L http://cpanmin.us | perl - App::cpanminus \
#     && cpanm Log::Dispatch::File \
#     && cpanm YAML::Tiny \
#     && cpanm File::HomeDir \
#     && cpanm Unicode::GCString

# Set environment variables
ENV LANG=C.UTF-8 \
    LC_ALL=C.UTF-8