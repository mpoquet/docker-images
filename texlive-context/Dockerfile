FROM nixos/nix:2.3
RUN nix-channel --remove nixpkgs \
 && nix-env -f https://github.com/NixOS/nixpkgs/archive/19.09.tar.gz -iA \
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
      texlive.combined.scheme-context \
 && nix-collect-garbage -d \
 && ln -s $(realpath $(which bash)) /bin/bash
