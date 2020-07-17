# Maintainer: Lone_Wolf <lone_wolf@klaas-de-kat.nl>
# Contributor: Armin K. <krejzi at email dot com>
# Contributor: Kristian Klausen <klausenbusk@hotmail.com>
# Contributor: Egon Ashrafinia <e.ashrafinia@gmail.com>
# Contributor: Tavian Barnes <tavianator@gmail.com>
# Contributor: Jan de Groot <jgc@archlinux.org>
# Contributor: Andreas Radke <andyrtr@archlinux.org>
# Contributor: Thomas Dziedzic < gostrc at gmail >
# Contributor: Antti "Tera" Oja <antti.bofh@gmail.com>
# Contributor: Diego Jose <diegoxter1006@gmail.com>

pkgname=mesa-git
pkgdesc="an open-source implementation of the OpenGL specification, git version"
pkgver=20.2.0_devel.126223.2b796c76852
pkgrel=1
arch=('x86_64')
makedepends=('git' 'python-mako' 'xorgproto'
              'libxml2' 'libx11'  'libvdpau' 'libva' 'elfutils' 'libomxil-bellagio' 'libxrandr'
              'ocl-icd' 'libgcrypt'  'wayland' 'wayland-protocols' 'meson' 'ninja')
depends=('libdrm' 'libxxf86vm' 'libxdamage' 'libxshmfence' 'libelf'
         'libomxil-bellagio' 'libunwind' 'libglvnd' 'wayland' 'lm_sensors' 'libclc' 'glslang' 'vulkan-icd-loader' 'zstd')
optdepends=('opengl-man-pages: for the OpenGL API man pages')
provides=('mesa' 'opencl-mesa' 'vulkan-intel' 'vulkan-radeon' 'vulkan-mesa-layer' 'libva-mesa-driver' 'mesa-vdpau' 'vulkan-driver' 'opengl-driver' 'opencl-driver')
conflicts=('mesa' 'opencl-mesa' 'vulkan-intel' 'vulkan-radeon' 'vulkan-mesa-layer' 'libva-mesa-driver' 'mesa-vdpau')
url="https://www.mesa3d.org"
license=('custom')
source=('mesa::git+https://gitlab.freedesktop.org/mesa/mesa.git'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5728.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5865.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5949.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5945.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5927.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5924.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5923.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5951.diff'
                'https://gitlab.freedesktop.org/pepp/mesa/-/commit/d71ff5b42cab85817e5c22c5e21eeaca87e39dec.diff'
                'LICENSE')
md5sums=('SKIP'
         'f5790c785525365eb9a46fe48812c6aa'
         '39b15400e0cfe98a1217a916141175d1'
         'cd87eeb820788224d770cb0073e1f196'
         '5f2a47e4a59f2cea37593be214cc26e9'
         '01793a514153eb50721d59b7a92316a7'
         'd16332b2811550208a64e768aa9701c7'
         'f45194ce4905ac462682b4302ec625a3'
         '3686cabf24a30c7331f20844a8f27b3d'
         'd92c6a427f007f563516f01f84358283'
         '5c65a0fe315dd347e09b1f2826a1df5a')
sha512sums=('SKIP'
            '889565e9a5cc4b1564fab1156b0a88b77e9802d56a5792b315d2552812c4eb478682b9f7046b89c0e41cd2492f768bd009ec2d5bf570fb42345910c4fe0d28b4'
            '8b44b83b9341b7ed8a59bdce250343cb2a71f0cd5c7d72afcfc892d3f83e93b53683c0da7862b01c28a5014576e09f214017626b92b820f92caf792cd1eab37d'
            '07a85825e7cfd61e4aa0ebae519cc0febc48798eb8b596ea9b63721d8045b6168980beeef6986aea120ab853ba4053dac6368c956bd18f5de90e58e42723dac2'
            '3b432ef147b15f85f144472c394a83b311c0dbae7818776c99a510d133e641411eff994f5e96fe2cb4d01ba9cea3181266784ece3f592f96141806e8fefe1ec1'
            'c4f02f2dc04feda956af62f96ce95760561d911805b3576dc311f9c007499ac6292140d41b583fcbfaf8b09e338c38cc4dc3e80e18fc25824f5e2fd0769a7db6'
            '79dbe9d4c5f24a97acb1d445bf47d9dd351ca61036e0d6ffdba3e51ac736699afb6bae7a1d327776690ae3261acd520dd0fde171b4b2f991f0a2063398bfc3c7'
            '8e5424486c01b1cedef3d124390496328bf322c174ceda67e5f4440f41403180fe8cbacb2d158dbd45f2f406d6ed7d54458199089934f20bf113a50849c2e36a'
            '7870cbe6e77ab2436b0ac647f6acbb0405fea17ffe382f2bd96de12a323469742d0be577874956684b708fdd1da6c0ae087aa74c630bff1a79f4b07d83e314e9'
            '37e3630ce56d003044168f25c54f65d84e78df386a5405fd1936a3754e85125c64db7fb235d202d578ee8b7e4c736a86632658eb2badb54ac7602d0f248e2783'
            '25da77914dded10c1f432ebcbf29941124138824ceecaf1367b3deedafaecabc082d463abcfa3d15abff59f177491472b505bcb5ba0c4a51bb6b93b4721a23c2')

# NINJAFLAGS is an env var used to pass commandline options to ninja
# NOTE: It's your responbility to validate the value of $NINJAFLAGS. If unsure, don't set it.

# MESA_WHICH_LLVM is an environment variable that determines which llvm package tree is used to built mesa-git against.
# Adding a line to ~/.bashrc  that sets this value is the simplest way to ensure a specific choice.
#
# NOTE: Aur helpers don't handle this method well, check the sticky comments on mesa-git aur page .
#
# 1: llvm-minimal-git (aur) preferred value
# 2: AUR llvm-git
# 3: llvm-git from LordHeavy unofficial repo 
# 4  llvm (stable from extra) Default value
# 

if [[ ! $MESA_WHICH_LLVM ]] ; then
    MESA_WHICH_LLVM=4
fi

case $MESA_WHICH_LLVM in
    1)
        # aur llvm-minimal-git
        makedepends+=('llvm-minimal-git')
        depends+=('llvm-libs-minimal-git')
        optdepends+=('llvm-minimal-git: opencl')
        ;;
    2)
        # aur llvm-git
        # depending on aur-llvm-* to avoid mixup with LH llvm-git
        makedepends+=('aur-llvm-git')
        depends+=('aur-llvm-libs-git')
        optdepends+=('llvm-git: opencl')
        ;;
    3)
        # mesa-git/llvm-git (lordheavy unofficial repo)
        makedepends+=('llvm-git' 'clang-git')
        depends+=('llvm-libs-git')
        optdepends+=('clang-git: opencl' 'compiler-rt: opencl')
        ;;
    4)
        # extra/llvm
        makedepends+=(llvm=10.0.0 clang=10.0.0)
        depends+=(llvm-libs=10.0.0)
        optdepends+=('clang: opencl' 'compiler-rt: opencl')
        ;;
    *)
esac
        
        
        
        
        
pkgver() {
    cd mesa
    read -r _ver <VERSION
    echo ${_ver/-/_}.$(git rev-list --count HEAD).$(git rev-parse --short HEAD)
}

prepare() {
    # although removing _build folder in build() function feels more natural,
    # that interferes with the spirit of makepkg --noextract
    if [  -d _build ]; then
        rm -rf _build
    fi
    cd "${srcdir}/mesa"
    patch -p1 < "${srcdir}/5865.diff"
    patch -p1 < "${srcdir}/5949.diff"
    patch -p1 < "${srcdir}/5945.diff"
    patch -p1 < "${srcdir}/5927.diff"
    patch -p1 < "${srcdir}/5924.diff"
    patch -p1 < "${srcdir}/5923.diff"
    patch -p1 < "${srcdir}/5951.diff"
    patch -p1 < "${srcdir}/d71ff5b42cab85817e5c22c5e21eeaca87e39dec.diff"
    patch -p1 -R < "${srcdir}/5728.diff"

}

build () {
    meson setup mesa _build \
       -D b_ndebug=true \
       -D b_lto=false \
       -D buildtype=plain \
       --wrap-mode=nofallback \
       -D prefix=/usr \
       -D sysconfdir=/etc \
       -D platforms=x11,wayland,drm,surfaceless \
       -D dri-drivers=i915,i965,r200,r100,nouveau \
       -D gallium-drivers=r300,r600,radeonsi,nouveau,svga,swrast,virgl,iris,zink \
       -D vulkan-drivers=amd,intel \
       -D dri3=enabled \
       -D egl=enabled \
       -D gallium-extra-hud=true \
       -D gallium-nine=true \
       -D gallium-omx=bellagio \
       -D gallium-va=enabled \
       -D gallium-vdpau=enabled \
       -D gallium-xa=enabled \
       -D gallium-xvmc=disabled \
       -D gbm=enabled \
       -D gles1=disabled \
       -D gles2=enabled \
       -D glvnd=true \
       -D glx=dri \
       -D libunwind=enabled \
       -D llvm=enabled \
       -D lmsensors=enabled \
       -D osmesa=gallium \
       -D shared-glapi=enabled \
       -D gallium-opencl=icd \
       -D valgrind=disabled \
       -D vulkan-overlay-layer=true \
       -D vulkan-device-select-layer=true \
       -D tools=[] \
       -D zstd=enabled \
       
    meson configure _build
    
    # quoted from https://www.mesa3d.org/meson.html
    # Note: autotools automatically updated translation files (used by the DRI configuration tool) as part of the build process, Meson does not do this. 
    # Instead, you will need do this: 
    # ninja $NINJAFLAGS -C _build xmlpool-pot xmlpool-update-po xmlpool-gmo
    # mesa devs handle driconf translation differently now, above command is no longer needed
    ninja $NINJAFLAGS -C _build
}

package() {
    DESTDIR="${pkgdir}" ninja $NINJAFLAGS -C _build install

    # remove script file from /usr/bin
    # https://gitlab.freedesktop.org/mesa/mesa/issues/2230
    rm "${pkgdir}/usr/bin/mesa-overlay-control.py"
    rmdir "${pkgdir}/usr/bin"
    
    # indirect rendering
    ln -s /usr/lib/libGLX_mesa.so.0 "${pkgdir}/usr/lib/libGLX_indirect.so.0"
  
    install -Dt "${pkgdir}/usr/share/licenses/${pkgname}" "${srcdir}/LICENSE"
}
