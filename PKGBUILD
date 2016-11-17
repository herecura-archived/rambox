#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.4.5
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha256sums_i686=('39d1de98cdbab21861deb17bf5d3ffff42ff7d05f3a2de5d4d2fc0d7f0f39a13')
sha256sums_x86_64=('e7ac1f1ff58ce69dd7ba0c41f840ed39d533eece719f9eba2f129ede96273ff0')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/Rambox "$pkgdir/usr/bin/rambox"
}
