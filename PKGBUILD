# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-fish-config
pkgver=1.0
pkgrel=1
pkgdesc="Fish configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'fish'
    'starship'
)
source=('.config')
optdepends=('stratos-starship-config: Starship configuration'
            'ttf-jetbrains-mono-nerd: Default nerd font')
install=stratos-fish-config.install
md5sums=('SKIP')
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/fish/" "$pkgdir/etc/skel/.config/"
}
