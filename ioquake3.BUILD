cc_binary(
    name = "ioq3ded",
    srcs = [
        "code/asm/ftola.c",
        "code/asm/qasm-inline.h",
        "code/asm/snapvector.c",
        "code/botlib/aasfile.h",
        "code/botlib/be_aas.h",
        "code/botlib/be_aas_bsp.h",
        "code/botlib/be_aas_bspq3.c",
        "code/botlib/be_aas_cluster.c",
        "code/botlib/be_aas_cluster.h",
        "code/botlib/be_aas_debug.c",
        "code/botlib/be_aas_debug.h",
        "code/botlib/be_aas_def.h",
        "code/botlib/be_aas_entity.c",
        "code/botlib/be_aas_entity.h",
        "code/botlib/be_aas_file.c",
        "code/botlib/be_aas_file.h",
        "code/botlib/be_aas_funcs.h",
        "code/botlib/be_aas_main.c",
        "code/botlib/be_aas_main.h",
        "code/botlib/be_aas_move.c",
        "code/botlib/be_aas_move.h",
        "code/botlib/be_aas_optimize.c",
        "code/botlib/be_aas_optimize.h",
        "code/botlib/be_aas_reach.c",
        "code/botlib/be_aas_reach.h",
        "code/botlib/be_aas_route.c",
        "code/botlib/be_aas_route.h",
        "code/botlib/be_aas_routealt.c",
        "code/botlib/be_aas_routealt.h",
        "code/botlib/be_aas_sample.c",
        "code/botlib/be_aas_sample.h",
        "code/botlib/be_ai_char.c",
        "code/botlib/be_ai_char.h",
        "code/botlib/be_ai_chat.c",
        "code/botlib/be_ai_chat.h",
        "code/botlib/be_ai_gen.c",
        "code/botlib/be_ai_gen.h",
        "code/botlib/be_ai_goal.c",
        "code/botlib/be_ai_goal.h",
        "code/botlib/be_ai_move.c",
        "code/botlib/be_ai_move.h",
        "code/botlib/be_ai_weap.c",
        "code/botlib/be_ai_weap.h",
        "code/botlib/be_ai_weight.c",
        "code/botlib/be_ai_weight.h",
        "code/botlib/be_ea.c",
        "code/botlib/be_ea.h",
        "code/botlib/be_interface.c",
        "code/botlib/be_interface.h",
        "code/botlib/botlib.h",
        "code/botlib/l_crc.c",
        "code/botlib/l_crc.h",
        "code/botlib/l_libvar.c",
        "code/botlib/l_libvar.h",
        "code/botlib/l_log.c",
        "code/botlib/l_log.h",
        "code/botlib/l_memory.c",
        "code/botlib/l_memory.h",
        "code/botlib/l_precomp.c",
        "code/botlib/l_precomp.h",
        "code/botlib/l_script.c",
        "code/botlib/l_script.h",
        "code/botlib/l_struct.c",
        "code/botlib/l_struct.h",
        "code/botlib/l_utils.h",
        "code/game/bg_public.h",
        "code/game/g_public.h",
        "code/null/null_client.c",
        "code/null/null_input.c",
        "code/null/null_snddma.c",
        "code/qcommon/cm_load.c",
        "code/qcommon/cm_local.h",
        "code/qcommon/cm_patch.c",
        "code/qcommon/cm_patch.h",
        "code/qcommon/cm_polylib.c",
        "code/qcommon/cm_polylib.h",
        "code/qcommon/cm_public.h",
        "code/qcommon/cm_test.c",
        "code/qcommon/cm_trace.c",
        "code/qcommon/cmd.c",
        "code/qcommon/common.c",
        "code/qcommon/cvar.c",
        "code/qcommon/files.c",
        "code/qcommon/huffman.c",
        "code/qcommon/ioapi.c",
        "code/qcommon/ioapi.h",
        "code/qcommon/md4.c",
        "code/qcommon/msg.c",
        "code/qcommon/net_chan.c",
        "code/qcommon/net_ip.c",
        "code/qcommon/q_math.c",
        "code/qcommon/q_platform.h",
        "code/qcommon/q_shared.c",
        "code/qcommon/q_shared.h",
        "code/qcommon/qcommon.h",
        "code/qcommon/qfiles.h",
        "code/qcommon/surfaceflags.h",
        "code/qcommon/unzip.c",
        "code/qcommon/unzip.h",
        "code/qcommon/vm.c",
        "code/qcommon/vm_interpreted.c",
        "code/qcommon/vm_local.h",
        "code/qcommon/vm_x86.c",
        "code/server/server.h",
        "code/server/sv_bot.c",
        "code/server/sv_ccmds.c",
        "code/server/sv_client.c",
        "code/server/sv_game.c",
        "code/server/sv_init.c",
        "code/server/sv_main.c",
        "code/server/sv_net_chan.c",
        "code/server/sv_snapshot.c",
        "code/server/sv_world.c",
        "code/sys/con_log.c",
        "code/sys/con_tty.c",
        "code/sys/sys_autoupdater.c",
        "code/sys/sys_loadlib.h",
        "code/sys/sys_local.h",
        "code/sys/sys_main.c",
        "code/sys/sys_unix.c",
        "code/zlib/adler32.c",
        "code/zlib/crc32.c",
        "code/zlib/crc32.h",
        "code/zlib/inffast.c",
        "code/zlib/inffast.h",
        "code/zlib/inffixed.h",
        "code/zlib/inflate.c",
        "code/zlib/inflate.h",
        "code/zlib/inftrees.c",
        "code/zlib/inftrees.h",
        "code/zlib/zconf.h",
        "code/zlib/zlib.h",
        "code/zlib/zutil.c",
        "code/zlib/zutil.h",
    ],
    copts = ["-Wno-return-type"],
    defines = [
        "ARCH_STRING=\\\"x86_64\\\"",
        "BOTLIB",
        "DEDICATED",
    ],
    linkopts = ["-ldl"],
    visibility = ["//visibility:public"],
)
