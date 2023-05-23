# Copyright 2023 DreamWorks Animation LLC
# SPDX-License-Identifier: Apache-2.0

add_subdirectory(geom)
add_subdirectory(lpe)
add_subdirectory(mcrt_common)
# TODO:
# /usr/bin/ld: ../../../../lib/rendering/pbr/librendering_pbr.so: undefined reference to `isRenderCanceled'
# add_subdirectory(pbr)
add_subdirectory(rndr)
# TODO:
# /usr/bin/ld: ../../../../lib/rendering/rt/librendering_rt.so: undefined reference to `vtable for moonray::pbr::ProjectiveCamera'
# /usr/bin/ld: ../../../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::PerspectiveCamera::PerspectiveCamera(scene_rdl2::rdl2::Camera const*)'
# /usr/bin/ld: ../../../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::ImageDistribution::~ImageDistribution()'
# /usr/bin/ld: ../../../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::Camera::update(scene_rdl2::math::Mat4<scene_rdl2::math::Vec4<double> > const&)'
# /usr/bin/ld: ../../../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::PerspectiveCamera::computeFrustumImpl(moonray::mcrt_common::Frustum*, float, bool) const'
# add_subdirectory(rt)
add_subdirectory(shading)
