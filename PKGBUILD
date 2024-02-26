# Maintainer: Neptune <neptune650@proton.me>
# Contributor: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Dag Odenhall <dag.odenhall@gmail.com>
# Contributor: Grigorios Bouzakis <grbzks@gmail.com>

pkgname=dwm
pkgver=6.4
pkgrel=1
pkgdesc="A dynamic window manager for X"
url="https://dwm.suckless.org"
arch=('i686' 'x86_64' 'arm' 'armv7h' 'armv6h' 'aarch64')
license=('MIT')
options=(zipman)
depends=('libx11' 'libxinerama' 'libxft' 'freetype2')
source=($pkgname::git+https://github.com/bx-sa1/dwm)

build() {
  cd "$srcdir/$pkgname"
  make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11 FREETYPEINC=/usr/include/freetype2
}

package() {
  cd "$srcdir/$pkgname"
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  install -Dm644 README "$pkgdir/usr/share/doc/$pkgname/README"
}


sha256sums=('SKIP'
            '87d65e2c786d98efca85a89979dcd74eef9217334fbc25c68a342f7c0aa531b4'
            'e5e205b9286b8b65821ee60fe8dc93bfd686c39cc6c07cdd82af52a824825d06')
sha256sums=('SKIP'
            '87d65e2c786d98efca85a89979dcd74eef9217334fbc25c68a342f7c0aa531b4'
            '7dbe9aa84f3b04d070be434a952c8f9ca6b65cf1dea88cd82680dfe382654e5a')
sha256sums=('SKIP'
            '87d65e2c786d98efca85a89979dcd74eef9217334fbc25c68a342f7c0aa531b4'
            '6365e5a742306ca64fec80cc1823fd6cedbf363d803e4830c9d8d4f508afc507')
sha256sums=('SKIP'
            '87d65e2c786d98efca85a89979dcd74eef9217334fbc25c68a342f7c0aa531b4'
            '6365e5a742306ca64fec80cc1823fd6cedbf363d803e4830c9d8d4f508afc507'
            '945a71e2822becfa37bc56c1a5e657a7142db54be69fbf8ab9e898e197c02cc9')
