#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.8
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('8e5ebd9c3089814e2c05ebc689d612c79560b9d671cf5e3451f6fca09c2c3aa7b756b4af0752c7d9cfddbb7fd43d8dc6d879e66b977b6cccdf5e79c0261237c2')
sha512sums_x86_64=('71af69b36756f1a9f2a5a30d0f3e8f3574d30ba4e9b8bd0da61cae9a8668a351e586e6baa66e9fb81bded99d73c8cf6eb60346b456c1281cfc3a3dfde4dac033')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
