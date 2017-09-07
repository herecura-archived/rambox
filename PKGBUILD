#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.12
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('1467cb7e48b56fe38c21b47a02ed2657c13c40a32b614a430e014e6b6d4908077df96b8eec0c324229372c9d846d1df661c01bcddb76e069cde59d0ea4907d2e')
sha512sums_x86_64=('e2342263c446b3d80c64a71728ff6efe029bf7b7634428bdf3eab8a9c3f500eeb66995847fc802be69d42cb8323094d0f036a07ff274e41144ac38eb6c3e03c0')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
