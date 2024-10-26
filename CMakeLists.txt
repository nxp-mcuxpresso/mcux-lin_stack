# Copyright 2024 NXP
# SPDX-License-Identifier: BSD-3-Clause

if(CONFIG_MCUX_COMPONENT_middleware.lin_stack)
    mcux_add_source(
        SOURCES coreapi/lin_common_api.c
                coreapi/lin_common_proto.c
                coreapi/lin_common_proto.h
                coreapi/lin_j2602_proto.c
                coreapi/lin_j2602_proto.h
                coreapi/lin_lin21_proto.c
                coreapi/lin_lin21_proto.h
                diagnostic/lin_diagnostic_service.c
                include/lin.h
                include/lin_common_api.h
                include/lin_commontl_api.h
                include/lin_diagnostic_service.h
                include/lin_types.h
                lowlevel/lin.c
                transport/lin_commontl_api.c
                transport/lin_commontl_proto.c
                transport/lin_commontl_proto.h
    )
    mcux_add_include(
        INCLUDES coreapi
                 include
                 transport
    )
endif()
