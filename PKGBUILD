#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.10
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('3031a654c20057afc7a419390c8cce0e35dc8a83b435ad49af2261aa0919fbfc756d26d24aec147f7316f57ddd74b5cfbd2a167af93dea5a2c1d611e093ab562')
sha512sums_x86_64=('47f06f7eefa5387426d6fd85b3a05c6ca5325cbd429997f1da9ea194447542ffe1defc858b12dad32b63c42b47d6cc16f19f957898eb995a213ba005bdb92f1f')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
