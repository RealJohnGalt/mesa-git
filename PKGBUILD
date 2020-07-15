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
pkgver=20.2.0_devel.126128.a9c94861063
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
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5869.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5868.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5728.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5863.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5865.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5899.diff'
                'https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests/5896.diff'
                'LICENSE')
md5sums=('SKIP'
         'a3ad2c21f98bd929deaf43c34338032d'
         '5a27fa6601abcc394a8b2222cfdf9d78'
         'f5790c785525365eb9a46fe48812c6aa'
         '81f010c2a02355017af2a8349fafa8df'
         '39b15400e0cfe98a1217a916141175d1'
         '1783918ef1cbc213ed5a3c4fe9882a26'
         '6fd950923f8da7ea904437a8ca5e8b55'
         '5c65a0fe315dd347e09b1f2826a1df5a')
sha512sums=('SKIP'
            '11ec2818560b55b18962c5b5dd940906d0e0762b6d0204c62a9c9bdd08887603ebe2b7efa9a404dc4f7940e5df00d6a8d1dc233d77029fe0c44ea5bc84640812'
            '3b026fce5747f11c155ce5537742e6f82c3a4ac9c747d1bc2aa4d4dea1f735590c2d455a7d3dbb27a05020d9a3948063a76bf8f9f834cc9627e1e7c34e096d8f'
            '889565e9a5cc4b1564fab1156b0a88b77e9802d56a5792b315d2552812c4eb478682b9f7046b89c0e41cd2492f768bd009ec2d5bf570fb42345910c4fe0d28b4'
            '6fb877e0647aa1130353b3bffff03400510c59659de2d3653ed72e2741f485d29d06ea05ddd709a644b5bed2918721d29d1eac52f16f70edafa6e476b320224c'
            '8b44b83b9341b7ed8a59bdce250343cb2a71f0cd5c7d72afcfc892d3f83e93b53683c0da7862b01c28a5014576e09f214017626b92b820f92caf792cd1eab37d'
            '931f6bd8afa44d016546f4d849a09fc1a0f89fa40095a6a4d967e01344c0cac7757a62c6f1c23a6a589ac8c9073a05103370a0f4496de48a1f4ee19ae2c0b4e9'
            'b25dad451182bfa53b7915a82c250e72f93dd4416f0bc3bafc0a743fb8f78fddcd6e7f1ed3a0be76a8c2557a7673781a81becdfb4c6c9fcbd70d7326c8d58c02'
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
    patch -p1 < "${srcdir}/5899.diff"
    patch -p1 < "${srcdir}/5896.diff"
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
