# Copyright 2023 DreamWorks Animation LLC
# SPDX-License-Identifier: Apache-2.0

if (MOONRAY_BUILD_BRDF_CMDS)
    add_subdirectory(brdf_cmd)
endif()

if (MOONRAY_BUILD_POINT_GENERATION_CMDS)
    add_subdirectory(point_generation_cmd)
endif()

# add_subdirectory(denoise_cmd) 
# TODO: link errors
# /usr/bin/ld: ../../lib/rendering/rt/librendering_rt.so: undefined reference to `vtable for moonray::pbr::ProjectiveCamera'
# /usr/bin/ld: ../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::PerspectiveCamera::PerspectiveCamera(scene_rdl2::rdl2::Camera const*)'
# /usr/bin/ld: ../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::ImageDistribution::~ImageDistribution()'
# /usr/bin/ld: ../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::Camera::update(scene_rdl2::math::Mat4<scene_rdl2::math::Vec4<double> > const&)'
# /usr/bin/ld: ../../lib/rendering/rt/librendering_rt.so: undefined reference to `moonray::pbr::PerspectiveCamera::computeFrustumImpl(moonray::mcrt_common::Frustum*, float, bool) const'

add_subdirectory(raas_cmd)
