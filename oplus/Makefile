CANOE_BASE_DTB += ../qcom/canoe.dtb ../qcom/canoe-v2.dtb ../qcom/canoe-tp.dtb ../qcom/canoe-tp-v2.dtb ../qcom/alor.dtb \
	../qcom/alor-interposer.dtb ../qcom/alor-interposer-v2.dtb ../qcom/alorp.dtb
CANOE_APQ_BASE_DTB += ../qcom/canoep.dtb ../qcom/canoep-v2.dtb ../qcom/canoep-tp.dtb ../qcom/canoep-tp-v2.dtb

CANOE_BOARDS += \
	infiniti-24831-canoe-overlay-t0.dtbo \
	infiniti-24863-canoe-overlay-t0.dtbo \
	infiniti-24863-canoe-overlay-pre-t0.dtbo \
	infiniti-24831-canoe-overlay-pre-t0.dtbo \
	infiniti-24863-canoe-overlay-evb.dtbo \
	infiniti-24831-canoe-overlay-production.dtbo \
	infiniti-24863-canoe-overlay-production.dtbo \
	infiniti-24831-canoe-overlay-evb.dtbo

CANOE_BOARDS += macan-24855-alor-overlay.dtbo \
	macan-24877-alor-overlay-IN.dtbo \
	macan-24877-alor-overlay-EU-US.dtbo \
	macan-24855-alor-overlay-dvt2.dtbo \
	fairlady-25821-canoe-overlay.dtbo \
	fairlady-25821-canoe-overlay-evb3.dtbo \
	fairlady-25871-canoe-overlay.dtbo \
	fairlady-25871-canoe-overlay-evb3.dtbo

# realme GT8 Pro (lafa, project 24624 / 24776).
# Unlike the other projects above, lafa ships a single overlay that covers the
# whole oplus,hw-id range (EVB1..PVT1); the stock ROM splits the same content
# across two dtbo entries instead. See oplus/platform_map.bzl.
CANOE_BOARDS += lafa-24624-canoe-overlay.dtbo

dtb-y += $(CANOE_BASE_DTB) $(CANOE_APQ_BASE_DTB) $(CANOE_BOARDS)

always-y        := $(dtb-y)
subdir-y        := $(dts-dirs)
clean-files     := *.dtb *.dtbo
