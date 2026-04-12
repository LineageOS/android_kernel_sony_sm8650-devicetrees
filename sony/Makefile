PINEAPPLE_BASE_DTB += ../qcom/pineapple.dtb ../qcom/pineapple-v2.dtb ../qcom/cliffs.dtb ../qcom/cliffs7.dtb
PINEAPPLE_APQ_BASE_DTB += ../qcom/pineapplep.dtb ../qcom/pineapplep-v2.dtb

ifeq ($(CONFIG_MACH_SONY_PDX245),y)
SOMC_PINEAPPLE_BOARDS += pineapple-asahi-pdx245_generic-overlay.dtbo
endif

pineapple-overlays-dtb-y += $(SOMC_PINEAPPLE_BOARDS) $(PINEAPPLE_BASE_DTB) $(PINEAPPLE_APQ_BASE_DTB)
pineapple-dtb-y += $(SOMC_PINEAPPLE_BOARDS) $(PINEAPPLE_BASE_DTB) $(PINEAPPLE_APQ_BASE_DTB)
dtb-y += $(pineapple-dtb-y)

always-y	:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files	:= *.dtb *.dtbo
