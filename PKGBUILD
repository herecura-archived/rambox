#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.7
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('9953b223c5f4fd8bcc17be629b5ccfb9a5014e5bddf92ee4634982442b7697ae8bbf7c134916cefdf5093f52635af1f3bab6237cde0c82eb35d467177114a4b2')
sha512sums_x86_64=('171df0d9571fe5c32e8fcd5e5d71f34fef8434a6836008810162df6f8257e8bfd70434b7c7d1dbec92c501369b095edab7dfd6e9d1d39207ad30c5b6ada76dfe')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/Rambox "$pkgdir/usr/bin/rambox"
}
