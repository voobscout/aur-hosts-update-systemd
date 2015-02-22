# Maintainer: Voobscout <voobscout+aur@gmail.com>
pkgname=hosts-update-systemd
pkgver=1.0.0
pkgrel=4
pkgdesc="AUR/hosts-update - systemd Timer"
arch=('any')
license=('MIT')
depends=('hosts-update')
url="https://aur.archlinux.org/packages/hosts-update"
provides=('hosts-update-systemd')
source=('hosts-update.service' 'hosts-update.timer')
sha256sums=('d601f8b21a3717ed6af310841988cf2e66f5a9fb946f05b7837b0a3ef24b1714'
            'd073b36c6d6021166b38117c99abccf49636660e236f8e28723be126c7a91e2b')
options=(!strip)
install=hosts-update-systemd.install

build() {
  msg2 "There isn't anything to build actually..."
}

package() {
  msg "Installing timer components..."
  install -Dm 0644 ${srcdir}/hosts-update.service ${pkgdir}/usr/lib/systemd/system/hosts-update.service
  install -Dm 0644 ${srcdir}/hosts-update.timer ${pkgdir}/usr/lib/systemd/system/hosts-update.timer
 }
