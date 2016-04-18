tion A :

0000000000600e50 d _DYNAMIC
0000000000600fe8 d _GLOBAL_OFFSET_TABLE_
0000000000400608 R _IO_stdin_used
                 w _Jv_RegisterClasses
00000000004004b4 T _Z7averagePdRd
00000000004004e2 T _Z7averageif
0000000000600e30 d __CTOR_END__
0000000000600e28 d __CTOR_LIST__
0000000000600e40 D __DTOR_END__
0000000000600e38 d __DTOR_LIST__
0000000000400738 r __FRAME_END__
0000000000600e48 d __JCR_END__
0000000000600e48 d __JCR_LIST__
0000000000601018 A __bss_start
0000000000601008 D __data_start
00000000004005c0 t __do_global_ctors_aux
0000000000400420 t __do_global_dtors_aux
0000000000601010 D __dso_handle
                 w __gmon_start__
0000000000600e24 d __init_array_end
0000000000600e24 d __init_array_start
00000000004005b0 T __libc_csu_fini
0000000000400520 T __libc_csu_init
                 U __libc_start_main@@GLIBC_2.2.5
0000000000601018 A _edata
0000000000601028 A _end
00000000004005f8 T _fini
0000000000400390 T _init
00000000004003d0 T _start
00000000004003fc t call_gmon_start
0000000000601018 b completed.6531
0000000000601008 W data_start
0000000000601020 b dtor_idx.6533
0000000000400490 t frame_dummy
000000000040050a T main



question B :

a : 1  pa : 8
b : 4  pb : 8
c : 4  pc : 8
d : 8  pd : 8

a b c d 分別是字元 整數 服點數 精確浮點數型別的資料
所以理所當然會用相對應的記憶體配置去存取
而pa pb pc pd 卻是指標的型別
指標本身是去儲存別的資料的位址
所以無論他是去存取哪種型別的資料位址
都是配置同樣大小的記憶體去存

