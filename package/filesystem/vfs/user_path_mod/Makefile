################################################
#
# user_path_mod
#
################################################
PK_USER_PATH_MOD_NAME        := user_path_mod
PK_USER_PATH_MOD_VERSION     := $(CONFIG_PK_USER_PATH_MOD_VERSION)
PK_USER_PATH_MOD_SITE        := $(CONFIG_PK_USER_PATH_MOD_URL)
PK_USER_PATH_MOD_GITHUB      := $(CONFIG_PK_USER_PATH_MOD_GITHUB)
PK_USER_PATH_MOD_SUBNAME     :=
PK_USER_PATH_MOD_BUILDARCH   := $(CONFIG_PK_USER_PATH_MOD_BUILDARCH)
PK_USER_PATH_MOD_DIR         := $(srctree)/package/filesystem/vfs/user_path_mode
PK_USER_PATH_MOD_PATCH       := $(PK_USER_PATH_MOD_DIR)/patch
PK_USER_PATH_MOD_BSBIT       := USER_PATH_MOD-$(PK_USER_PATH_MOD_VERSION).bsbit
PK_USER_PATH_MOD_OUT         :=
PK_USER_PATH_MOD_SCRIPTS     := $(srctree)/scripts/package/package-module.sh
PK_USER_PATH_MOD_TAR         := $(CONFIG_PK_USER_PATH_MOD_TAR)
PK_USER_PATH_MOD_PACKAGE     :=
PK_USER_PATH_MOD_CONFIG      := $(CONFIG_PK_USER_PATH_MOD_CONFIG)
SUB_TARGET                  += $(PK_USER_PATH_MOD_DIR)/build

PK_USER_PATH_MOD_sh = $(CONFIG_SHELL) $(PK_USER_PATH_MOD_SCRIPTS) \
                 $1X \
                 $(PK_USER_PATH_MOD_NAME)X \
                 $(PK_USER_PATH_MOD_VERSION)X \
                 $(PK_USER_PATH_MOD_SITE)X \
                 $(PK_USER_PATH_MOD_GITHUB)X \
                 $(PK_USER_PATH_MOD_PATCH)X \
                 $(CONFIG_LINUX_KERNEL_VERSION)X \
	         $(CONFIG_MAIN_PROJ_NAME)X \
                 $(PK_USER_PATH_MOD_TAR)X \
                 $(CONFIG_LINUX_KERNEL_CROSS_COMPILE)X \
                 $(PK_USER_PATH_MOD_SUBNAME)X \
                 $(CONFIG_PK_USER_PATH_MOD_CONFIG)X \
                 $(CONFIG_PK_USER_PATH_MOD_LIBPATH)X \
                 $(CONFIG_PK_USER_PATH_MOD_CPPFLAGS)X \
                 $(CONFIG_PK_USER_PATH_MOD_DPKCONFIG)X \
                 $(CONFIG_PK_USER_PATH_MOD_CFLAGS)X \
                 $(CONFIG_PK_USER_PATH_MOD_LDFLAGS)X \
                 $(CONFIG_PK_USER_PATH_MOD_CXXFLAGS)X \
                 $(CONFIG_PK_USER_PATH_MOD_ASFLAGS)X \
                 $(PK_USER_PATH_MOD_BSBIT)X \
                 $(PK_USER_PATH_MOD_BUILDARCH)X \
		 $(PK_USER_PATH_MOD_CSRCFILE)X \
                 $(CONFIG_PK_USER_PATH_MOD_SRCFILE)X \
                 $(CONFIG_PK_USER_PATH_MOD_CSRCFILE)

$(PK_USER_PATH_MOD_DIR)/build: FORCE
	$(Q)$(call PK_USER_PATH_MOD_sh,$(srctree))
