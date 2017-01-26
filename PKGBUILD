#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.2
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha256sums_i686=('06d88f701f9b2a5ce6b144469b11fb0dc76a8e2a174c1dc2a082ddc123973ebf')
sha256sums_x86_64=('0f6c389da26b85fbcaa0e5a83fc1ba7e889cc8defd3581ef91f271a143c09742')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/Rambox "$pkgdir/usr/bin/rambox"
}
