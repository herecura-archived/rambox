#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.3
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha256sums_i686=('cf1b102f393bde402a9d1b3a5557758e8fe6c820f0d588b656a66a2919f5c175')
sha256sums_x86_64=('3067f75b86337e5518299135963e25d280e8ec917d95b8db01f662b70c4d2a75')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/Rambox "$pkgdir/usr/bin/rambox"
}
