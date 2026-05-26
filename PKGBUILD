pkgname=keskos-mirrorlist
pkgver=0.1.0
pkgrel=1
pkgdesc="KeskOS pacman mirrorlist"
arch=(any)
url="https://github.com/memegeko/keskos"
license=(custom:KeskOS)
backup=(etc/pacman.d/keskos-mirrorlist)
source=()
sha256sums=()

package() {
  install -d "${pkgdir}/etc/pacman.d"
  cat >"${pkgdir}/etc/pacman.d/keskos-mirrorlist" <<'EOF'
Server = https://downloads.keskos.org/repo/$repo/os/$arch
EOF
}
