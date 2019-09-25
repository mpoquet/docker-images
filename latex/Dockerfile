FROM nixos/nix:2.2.1
RUN nix-channel --remove nixpkgs \
 && nix-env -f https://github.com/NixOS/nixpkgs/archive/19.03.tar.gz -iA \
      bash \
      coreutils \
      curl \
      gitMinimal \
      gnutar \
      gzip \
      openssh \
      rsync \
      which \
      xz \
      texlive.combined.scheme-full \
 && nix-collect-garbage -d \
 && ln -s $(realpath $(which bash)) /bin/bash
