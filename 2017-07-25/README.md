`id:000000,sig:06,src:000071+000112,op:splice,rep:4`
```
#0  __GI_raise (sig=sig@entry=6) at ../sysdeps/unix/sysv/linux/raise.c:51
#1  0x00007f94219dc3fa in __GI_abort () at abort.c:89
#2  0x00007f9422bc760a in free (ptr=<optimized out>) at libdislocator.so.c:212
#3  0x00007f942297364f in opj_t1_allocate_buffers (t1=0x7f940ecdaf00, w=<optimized out>, h=<optimized out>) at /root/openjpeg/src/lib/openjp2/t1.c:1502
#4  0x00007f9422966429 in opj_t1_decode_cblk (t1=<optimized out>, cblk=<optimized out>, orient=<optimized out>, roishift=0, cblksty=48)
    at /root/openjpeg/src/lib/openjp2/t1.c:1791
#5  opj_t1_clbl_decode_processor (user_data=<optimized out>, tls=<optimized out>) at /root/openjpeg/src/lib/openjp2/t1.c:1652
#6  0x00007f942290afc1 in opj_thread_pool_submit_job (tp=0x7f9422eb9fa8, job_fn=0x7f9422966240 <opj_t1_clbl_decode_processor>, user_data=0x7f940ecd4fd0)
    at /root/openjpeg/src/lib/openjp2/thread.c:828
#7  0x00007f9422965fc6 in opj_t1_decode_cblks (tp=<optimized out>, pret=<optimized out>, tilec=<optimized out>, tccp=<optimized out>)
    at /root/openjpeg/src/lib/openjp2/t1.c:1763
#8  0x00007f94229b0c6f in opj_tcd_t1_decode (p_tcd=<optimized out>) at /root/openjpeg/src/lib/openjp2/tcd.c:1693
#9  opj_tcd_decode_tile (p_tcd=<optimized out>, p_src=<optimized out>, p_max_length=<optimized out>, p_tile_no=<optimized out>, p_cstr_index=<optimized out>,
    p_manager=<optimized out>) at /root/openjpeg/src/lib/openjp2/tcd.c:1425
#10 0x00007f942292b2de in opj_j2k_decode_tile (p_j2k=<optimized out>, p_tile_index=2, p_data=<optimized out>, p_data_size=<optimized out>, p_stream=<optimized out>,
    p_manager=<optimized out>) at /root/openjpeg/src/lib/openjp2/j2k.c:8649
#11 0x00007f94229400db in opj_j2k_decode_tiles (p_j2k=<optimized out>, p_stream=<optimized out>, p_manager=<optimized out>)
    at /root/openjpeg/src/lib/openjp2/j2k.c:10348
#12 0x00007f942292ef81 in opj_j2k_exec (p_j2k=0x7f9422ecced0, p_procedure_list=<optimized out>, p_stream=0x7f9422fd7f88, p_manager=0x7f9422ed0fa8)
    at /root/openjpeg/src/lib/openjp2/j2k.c:7826
#13 opj_j2k_decode (p_j2k=<optimized out>, p_stream=<optimized out>, p_image=<optimized out>, p_manager=<optimized out>) at /root/openjpeg/src/lib/openjp2/j2k.c:10567
#14 0x00007f942294acf8 in opj_jp2_decode (jp2=0x7f9422ecef50, p_stream=0x7f9422fd7f88, p_image=0x7f9420f79fd0, p_manager=0x7f9422ed0fa8)
    at /root/openjpeg/src/lib/openjp2/jp2.c:1564
#15 0x00007f942295abb3 in opj_decode (p_codec=0x7f9422ed0f50, p_stream=0x7f9422fd7f88, p_image=0x7f9420f79fd0) at /root/openjpeg/src/lib/openjp2/openjpeg.c:441
#16 0x0000000000406575 in main (argc=<optimized out>, argv=<optimized out>) at /root/openjpeg/src/bin/jp2/opj_decompress.c:1460
```


`id:000001,sig:06,src:000088,op:havoc,rep:2`
```
#0  __GI_raise (sig=sig@entry=6) at ../sysdeps/unix/sysv/linux/raise.c:51
#1  0x00007faa3a9793fa in __GI_abort () at abort.c:89
#2  0x00007faa3bb6460a in free (ptr=<optimized out>) at libdislocator.so.c:212
#3  0x00007faa3b949f02 in opj_tcd_free_tile (p_tcd=<optimized out>) at /root/openjpeg/src/lib/openjp2/tcd.c:1634
#4  opj_tcd_destroy (tcd=<optimized out>) at /root/openjpeg/src/lib/openjp2/tcd.c:661
#5  0x00007faa3b8be871 in opj_j2k_destroy (p_j2k=0x7faa3be69ed0) at /root/openjpeg/src/lib/openjp2/j2k.c:8036
#6  0x00007faa3b8ec8c1 in opj_jp2_destroy (jp2=0x7faa3be6bf50) at /root/openjpeg/src/lib/openjp2/jp2.c:2948
#7  0x00007faa3b8f8bfd in opj_destroy_codec (p_codec=0x7faa3be6df50) at /root/openjpeg/src/lib/openjp2/openjpeg.c:885
#8  0x0000000000408d0e in main (argc=<optimized out>, argv=<optimized out>) at /root/openjpeg/src/bin/jp2/opj_decompress.c:1463
```


`id:000048,sig:11,src:000498,op:havoc,rep:4`
```
#0  0x00000000004095fe in clip_component (component=0x7dfd60, precision=8) at /root/openjpeg/src/bin/jp2/convert.c:88
#1  0x0000000000422d9e in imagetotif (image=<optimized out>, outfile=<optimized out>) at /root/openjpeg/src/bin/jp2/converttif.c:640
#2  0x0000000000408529 in main (argc=<optimized out>, argv=<optimized out>) at /root/openjpeg/src/bin/jp2/opj_decompress.c:1628
```


`id:000133,sig:11,src:000960,op:havoc,rep:4`
```
#0  0x000000000040984f in clip_component (component=0x184a950, precision=10) at /root/openjpeg/src/bin/jp2/convert.c:79
#1  0x0000000000422d9e in imagetotif (image=<optimized out>, outfile=<optimized out>) at /root/openjpeg/src/bin/jp2/converttif.c:640
#2  0x0000000000408529 in main (argc=<optimized out>, argv=<optimized out>) at /root/openjpeg/src/bin/jp2/opj_decompress.c:1628
```

