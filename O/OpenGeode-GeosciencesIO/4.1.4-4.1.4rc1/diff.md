# Comparing `tmp/OpenGeode_GeosciencesIO-4.1.4-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_GeosciencesIO-4.1.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 342344 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/__init__.py
--rw-rw-rw-  2.0 fat     1233 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/mesh.py
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/model.py
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
--rw-rw-rw-  2.0 fat   398336 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
--rw-rw-rw-  2.0 fat   125952 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jun-08 00:57 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3335 b- defN 23-Jun-08 00:57 OpenGeode_GeosciencesIO-4.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-08 00:57 OpenGeode_GeosciencesIO-4.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-08 00:57 OpenGeode_GeosciencesIO-4.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1145 b- defN 23-Jun-08 00:57 OpenGeode_GeosciencesIO-4.1.4.dist-info/RECORD
-11 files, 794238 bytes uncompressed, 340350 bytes compressed:  57.1%
+Zip file size: 342380 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/__init__.py
+-rw-rw-rw-  2.0 fat     1233 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/mesh.py
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/model.py
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
+-rw-rw-rw-  2.0 fat   398336 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
+-rw-rw-rw-  2.0 fat   125952 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Jun-07 15:03 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3344 b- defN 23-Jun-07 15:03 OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-07 15:03 OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-07 15:03 OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1157 b- defN 23-Jun-07 15:03 OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/RECORD
+11 files, 794259 bytes uncompressed, 340362 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
 Comment: 
 
 Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.1.4.dist-info/METADATA
+Filename: OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.1.4.dist-info/WHEEL
+Filename: OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.1.4.dist-info/top_level.txt
+Filename: OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.1.4.dist-info/RECORD
+Filename: OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001581c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Jun  8 00:57:27 2023
+Time/Date		Wed Jun  7 15:03:31 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000016600
 SizeOfInitializedData	000000000000ae00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001581c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00027000
 SizeOfHeaders		00000400
-CheckSum		0002317f
+CheckSum		00021b16
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -32704,29 +32704,32 @@
    180019473:	imul   $0x1e200000,0x6e(%rdi),%ebp
    18001947a:	add    0x1(%rax),%al
    180019480:	rcrb   $0x2,(%rsi)
    180019483:	addb   $0x0,(%rcx)
    180019486:	add    %al,(%rax)
    180019488:	add    %al,(%rax)
    18001948a:	add    %al,(%rax)
-   18001948c:	ja     0x1800194b5
-   18001948e:	andl   $0xd0000,0x0(%rax,%rax,1)
-   180019496:	add    %al,(%rax)
-   180019498:	sub    %al,(%rbx)
-   18001949a:	add    %al,(%rax)
-   18001949c:	call   0x16801964c
-   1800194a1:	xchg   %eax,%ebp
-   1800194a2:	add    %eax,(%rax)
+   18001948c:	rex.XB pushf
+   18001948e:	andb   $0x0,0x0(%rax,%rax,1)
+   180019493:	add    %cl,0x28000000(%rip)        # 0x1a8019499
+   180019499:	add    (%rax),%eax
+   18001949b:	add    %ch,%al
+   18001949d:	stos   %eax,%es:(%rdi)
+   18001949e:	add    %eax,(%rax)
+   1800194a0:	call   0x18001963a
 	...
-   1800194b0:	cmp    %al,(%rcx)
+   1800194ad:	add    %al,(%rax)
+   1800194af:	add    %bh,(%rax)
+   1800194b1:	add    %eax,(%rax)
 	...
-   180019506:	add    %al,(%rax)
-   180019508:	or     %dl,(%rax)
-   18001950a:	add    0x1(%rax),%al
+   180019507:	add    %cl,(%rax)
+   180019509:	adc    %al,(%rdx)
+   18001950b:	addb   $0x0,(%rcx)
 	...
+   18001951e:	add    %al,(%rax)
    180019520:	xor    %al,0x18001(%rbp)
    180019526:	add    %al,(%rax)
    180019528:	rex test %eax,(%rcx)
    18001952b:	addb   $0x0,(%rcx)
 	...
    18001953e:	add    %al,(%rax)
    180019540:	add    %al,(%rcx)
```

## opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004415c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Jun  8 00:57:46 2023
+Time/Date		Wed Jun  7 15:03:51 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000047000
 SizeOfInitializedData	000000000001a000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004415c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00065000
 SizeOfHeaders		00000400
-CheckSum		000637f0
+CheckSum		00064ee4
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -76287,15 +76287,15 @@
    18003af28:	lea    0x22c31(%rip),%r8        # 0x18005db60
    18003af2f:	xor    %edx,%edx
    18003af31:	call   0x180044854
    18003af36:	test   %rax,%rax
    18003af39:	jne    0x18003af54
    18003af3b:	mov    $0x198,%r8d
    18003af41:	lea    0xfae8(%rip),%rdx        # 0x18004aa30
-   18003af48:	lea    0xfb41(%rip),%rcx        # 0x18004aa90
+   18003af48:	lea    0xfb49(%rip),%rcx        # 0x18004aa98
    18003af4f:	call   0x18003ed1a
    18003af54:	movupd 0x18(%rbx),%xmm0
    18003af59:	movdqa %xmm0,-0x49(%rbp)
    18003af5e:	lea    -0x49(%rbp),%rdx
    18003af62:	mov    %rsi,%rcx
    18003af65:	call   0x18004330a
    18003af6a:	lea    -0x69(%rbp),%rcx
@@ -76482,15 +76482,15 @@
    18003b215:	lea    0x22944(%rip),%r8        # 0x18005db60
    18003b21c:	xor    %edx,%edx
    18003b21e:	call   0x180044854
    18003b223:	test   %rax,%rax
    18003b226:	jne    0x18003b241
    18003b228:	mov    $0x198,%r8d
    18003b22e:	lea    0xf7fb(%rip),%rdx        # 0x18004aa30
-   18003b235:	lea    0xf854(%rip),%rcx        # 0x18004aa90
+   18003b235:	lea    0xf85c(%rip),%rcx        # 0x18004aa98
    18003b23c:	call   0x18003ed1a
    18003b241:	mov    0x20(%rdi),%r13
    18003b245:	movslq 0x18(%rdi),%rax
    18003b249:	lea    0x0(,%rax,8),%r12
    18003b251:	add    %r13,%r12
    18003b254:	mov    %r12,0x58(%rsp)
    18003b259:	cmp    %r12,%r13
@@ -76589,15 +76589,15 @@
    18003b3c6:	lea    0x22793(%rip),%r8        # 0x18005db60
    18003b3cd:	xor    %edx,%edx
    18003b3cf:	call   0x180044854
    18003b3d4:	test   %rax,%rax
    18003b3d7:	jne    0x18003b3f2
    18003b3d9:	mov    $0x198,%r8d
    18003b3df:	lea    0xf64a(%rip),%rdx        # 0x18004aa30
-   18003b3e6:	lea    0xf6a3(%rip),%rcx        # 0x18004aa90
+   18003b3e6:	lea    0xf6ab(%rip),%rcx        # 0x18004aa98
    18003b3ed:	call   0x18003ed1a
    18003b3f2:	mov    (%rdi),%rax
    18003b3f5:	mov    %rdi,%rcx
    18003b3f8:	call   *0x228(%rax)
    18003b3fe:	mov    (%rdi),%rcx
    18003b401:	mov    0x240(%rcx),%rdx
    18003b408:	mov    %rdi,%rcx
@@ -76868,15 +76868,15 @@
    18003b7cb:	lea    0x2238e(%rip),%r8        # 0x18005db60
    18003b7d2:	xor    %edx,%edx
    18003b7d4:	call   0x180044854
    18003b7d9:	test   %rax,%rax
    18003b7dc:	jne    0x18003b7f7
    18003b7de:	mov    $0x198,%r8d
    18003b7e4:	lea    0xf245(%rip),%rdx        # 0x18004aa30
-   18003b7eb:	lea    0xf29e(%rip),%rcx        # 0x18004aa90
+   18003b7eb:	lea    0xf2a6(%rip),%rcx        # 0x18004aa98
    18003b7f2:	call   0x18003ed1a
    18003b7f7:	mov    0x20(%rbx),%rcx
    18003b7fb:	mov    %rcx,0x40(%rsp)
    18003b800:	movslq 0x18(%rbx),%rax
    18003b804:	lea    (%rcx,%rax,8),%rax
    18003b808:	mov    %rax,-0x78(%rbp)
    18003b80c:	cmp    %rax,%rcx
@@ -76999,15 +76999,15 @@
    18003b9f0:	lea    0x22169(%rip),%r8        # 0x18005db60
    18003b9f7:	xor    %edx,%edx
    18003b9f9:	call   0x180044854
    18003b9fe:	test   %rax,%rax
    18003ba01:	jne    0x18003ba1c
    18003ba03:	mov    $0x198,%r8d
    18003ba09:	lea    0xf020(%rip),%rdx        # 0x18004aa30
-   18003ba10:	lea    0xf079(%rip),%rcx        # 0x18004aa90
+   18003ba10:	lea    0xf081(%rip),%rcx        # 0x18004aa98
    18003ba17:	call   0x18003ed1a
    18003ba1c:	mov    %r13,%r8
    18003ba1f:	mov    %rbx,%rdx
    18003ba22:	mov    %r14,%rcx
    18003ba25:	call   0x18003be10
    18003ba2a:	lea    0x38(%rsp),%rcx
    18003ba2f:	call   0x18003ed7a
@@ -78697,15 +78697,15 @@
    18003d2b3:	mov    %rsi,%rcx
    18003d2b6:	call   *0xb2ec(%rip)        # 0x1800485a8
    18003d2bc:	mov    $0x1,%r13d
    18003d2c2:	mov    %r13d,0x20(%rsp)
    18003d2c7:	mov    %rsi,%rdx
    18003d2ca:	lea    -0x20(%rbp),%rcx
    18003d2ce:	call   0x18003ec1e
-   18003d2d3:	lea    0xd80a(%rip),%r8        # 0x18004aae4
+   18003d2d3:	lea    0xd812(%rip),%r8        # 0x18004aaec
    18003d2da:	lea    0x1a0(%rbp),%rdx
    18003d2e1:	lea    0xf0(%rbx),%rcx
    18003d2e8:	call   0x18003fbc0
    18003d2ed:	mov    %rax,%rcx
    18003d2f0:	call   0x18003fc30
    18003d2f5:	mov    %rax,%r8
    18003d2f8:	mov    0xba79(%rip),%r10        # 0x180048d78
@@ -78757,19 +78757,19 @@
    18003d391:	mov    %rcx,0x30(%rsp)
    18003d396:	mov    %rdx,0x38(%rsp)
    18003d39b:	movaps 0x30(%rsp),%xmm0
    18003d3a0:	movdqa %xmm0,-0x50(%rbp)
    18003d3a5:	lea    -0x50(%rbp),%rdx
    18003d3a9:	lea    -0x8(%rbp),%rcx
    18003d3ad:	call   *0xb23d(%rip)        # 0x1800485f0
-   18003d3b3:	lea    0xd732(%rip),%r8        # 0x18004aaec
+   18003d3b3:	lea    0xd73a(%rip),%r8        # 0x18004aaf4
    18003d3ba:	lea    0x1a8(%rbp),%rdx
    18003d3c1:	lea    0xf0(%rbx),%rcx
    18003d3c8:	call   0x18003fbc0
-   18003d3cd:	lea    0xd724(%rip),%r8        # 0x18004aaf8
+   18003d3cd:	lea    0xd72c(%rip),%r8        # 0x18004ab00
    18003d3d4:	lea    0x1a0(%rbp),%rdx
    18003d3db:	lea    0x1a8(%rbp),%rcx
    18003d3e2:	call   0x18003fb50
    18003d3e7:	mov    %rax,%rcx
    18003d3ea:	call   0x180043250
    18003d3ef:	mov    %rax,0x30(%rsp)
    18003d3f4:	test   %rax,%rax
@@ -78816,15 +78816,15 @@
    18003d4b4:	call   0x18003f750
    18003d4b9:	test   %al,%al
    18003d4bb:	je     0x18003dd69
    18003d4c1:	lea    0x18(%rbp),%rcx
    18003d4c5:	call   0x180002a60
    18003d4ca:	mov    %rax,%rdi
    18003d4cd:	mov    %rax,0x10(%rbp)
-   18003d4d1:	lea    0xd60c(%rip),%r8        # 0x18004aae4
+   18003d4d1:	lea    0xd614(%rip),%r8        # 0x18004aaec
    18003d4d8:	lea    0xc0(%rbp),%rdx
    18003d4df:	mov    %rax,%rcx
    18003d4e2:	call   0x18003fbc0
    18003d4e7:	mov    %rax,%rcx
    18003d4ea:	call   0x18003fc30
    18003d4ef:	mov    %rax,%r8
    18003d4f2:	mov    0xb87f(%rip),%r10        # 0x180048d78
@@ -78906,15 +78906,15 @@
    18003d61f:	call   0x18003f750
    18003d624:	test   %al,%al
    18003d626:	je     0x18003d9ce
    18003d62c:	nopl   0x0(%rax)
    18003d630:	lea    0x60(%rsp),%rcx
    18003d635:	call   0x180002a60
    18003d63a:	mov    %rax,%rbx
-   18003d63d:	lea    0xd4a0(%rip),%r8        # 0x18004aae4
+   18003d63d:	lea    0xd4a8(%rip),%r8        # 0x18004aaec
    18003d644:	lea    0xc8(%rbp),%rdx
    18003d64b:	mov    %rax,%rcx
    18003d64e:	call   0x18003fbc0
    18003d653:	mov    %rax,%rcx
    18003d656:	call   0x18003fc30
    18003d65b:	mov    %rax,%r8
    18003d65e:	mov    0xb713(%rip),%r10        # 0x180048d78
@@ -79156,15 +79156,15 @@
    18003da10:	call   0x18003f750
    18003da15:	test   %al,%al
    18003da17:	je     0x18003dd47
    18003da1d:	nopl   (%rax)
    18003da20:	lea    0x60(%rsp),%rcx
    18003da25:	call   0x180002a60
    18003da2a:	mov    %rax,%rbx
-   18003da2d:	lea    0xd0b0(%rip),%r8        # 0x18004aae4
+   18003da2d:	lea    0xd0b8(%rip),%r8        # 0x18004aaec
    18003da34:	lea    0xd8(%rbp),%rdx
    18003da3b:	mov    %rax,%rcx
    18003da3e:	call   0x18003fbc0
    18003da43:	mov    %rax,%rcx
    18003da46:	call   0x18003fc30
    18003da4b:	mov    %rax,%r8
    18003da4e:	mov    0xb323(%rip),%r10        # 0x180048d78
@@ -79379,43 +79379,43 @@
    18003dd81:	pop    %r13
    18003dd83:	pop    %r12
    18003dd85:	pop    %rdi
    18003dd86:	pop    %rsi
    18003dd87:	pop    %rbx
    18003dd88:	pop    %rbp
    18003dd89:	ret
-   18003dd8a:	lea    0xcd37(%rip),%rcx        # 0x18004aac8
+   18003dd8a:	lea    0xcd3f(%rip),%rcx        # 0x18004aad0
    18003dd91:	call   0x1800433b2
    18003dd96:	nop
-   18003dd97:	lea    0xcd2a(%rip),%rcx        # 0x18004aac8
+   18003dd97:	lea    0xcd32(%rip),%rcx        # 0x18004aad0
    18003dd9e:	call   0x1800433b2
    18003dda3:	int3
    18003dda4:	lea    0xcd65(%rip),%rdx        # 0x18004ab10
    18003ddab:	lea    0x30(%rbp),%rcx
    18003ddaf:	call   0x180004380
    18003ddb4:	lea    0x1647d(%rip),%rdx        # 0x180054238
    18003ddbb:	lea    0x30(%rbp),%rcx
    18003ddbf:	call   0x180044848
    18003ddc4:	nop
    18003ddc5:	lea    0xc4b4(%rip),%rcx        # 0x18004a280
    18003ddcc:	call   0x1800433b2
    18003ddd1:	int3
-   18003ddd2:	lea    0xccef(%rip),%rcx        # 0x18004aac8
+   18003ddd2:	lea    0xccf7(%rip),%rcx        # 0x18004aad0
    18003ddd9:	call   0x1800433b2
    18003ddde:	int3
-   18003dddf:	lea    0xcce2(%rip),%rcx        # 0x18004aac8
+   18003dddf:	lea    0xccea(%rip),%rcx        # 0x18004aad0
    18003dde6:	call   0x1800433b2
    18003ddeb:	int3
    18003ddec:	lea    0xc48d(%rip),%rcx        # 0x18004a280
    18003ddf3:	call   0x1800433b2
    18003ddf8:	int3
-   18003ddf9:	lea    0xccc8(%rip),%rcx        # 0x18004aac8
+   18003ddf9:	lea    0xccd0(%rip),%rcx        # 0x18004aad0
    18003de00:	call   0x1800433b2
    18003de05:	int3
-   18003de06:	lea    0xccbb(%rip),%rcx        # 0x18004aac8
+   18003de06:	lea    0xccc3(%rip),%rcx        # 0x18004aad0
    18003de0d:	call   0x1800433b2
    18003de12:	int3
    18003de13:	int3
    18003de14:	int3
    18003de15:	int3
    18003de16:	int3
    18003de17:	int3
@@ -79445,15 +79445,15 @@
    18003de53:	mov    %rsi,%rcx
    18003de56:	call   *0xa73c(%rip)        # 0x180048598
    18003de5c:	mov    $0x1,%r13d
    18003de62:	mov    %r13d,0x20(%rsp)
    18003de67:	mov    %rsi,%rdx
    18003de6a:	lea    -0x20(%rbp),%rcx
    18003de6e:	call   0x18003ebf4
-   18003de73:	lea    0xcc6a(%rip),%r8        # 0x18004aae4
+   18003de73:	lea    0xcc72(%rip),%r8        # 0x18004aaec
    18003de7a:	lea    0x1a0(%rbp),%rdx
    18003de81:	lea    0xf0(%rbx),%rcx
    18003de88:	call   0x18003fbc0
    18003de8d:	mov    %rax,%rcx
    18003de90:	call   0x18003fc30
    18003de95:	mov    %rax,%r8
    18003de98:	mov    0xaed9(%rip),%r10        # 0x180048d78
@@ -79505,19 +79505,19 @@
    18003df31:	mov    %rcx,0x30(%rsp)
    18003df36:	mov    %rdx,0x38(%rsp)
    18003df3b:	movaps 0x30(%rsp),%xmm0
    18003df40:	movdqa %xmm0,-0x50(%rbp)
    18003df45:	lea    -0x50(%rbp),%rdx
    18003df49:	lea    -0x8(%rbp),%rcx
    18003df4d:	call   *0xa69d(%rip)        # 0x1800485f0
-   18003df53:	lea    0xcb92(%rip),%r8        # 0x18004aaec
+   18003df53:	lea    0xcb9a(%rip),%r8        # 0x18004aaf4
    18003df5a:	lea    0x1a8(%rbp),%rdx
    18003df61:	lea    0xf0(%rbx),%rcx
    18003df68:	call   0x18003fbc0
-   18003df6d:	lea    0xcb84(%rip),%r8        # 0x18004aaf8
+   18003df6d:	lea    0xcb8c(%rip),%r8        # 0x18004ab00
    18003df74:	lea    0x1a0(%rbp),%rdx
    18003df7b:	lea    0x1a8(%rbp),%rcx
    18003df82:	call   0x18003fb50
    18003df87:	mov    %rax,%rcx
    18003df8a:	call   0x180043250
    18003df8f:	mov    %rax,0x30(%rsp)
    18003df94:	test   %rax,%rax
@@ -79564,15 +79564,15 @@
    18003e054:	call   0x18003f750
    18003e059:	test   %al,%al
    18003e05b:	je     0x18003e909
    18003e061:	lea    0x18(%rbp),%rcx
    18003e065:	call   0x180002a60
    18003e06a:	mov    %rax,%rdi
    18003e06d:	mov    %rax,0x10(%rbp)
-   18003e071:	lea    0xca6c(%rip),%r8        # 0x18004aae4
+   18003e071:	lea    0xca74(%rip),%r8        # 0x18004aaec
    18003e078:	lea    0xc0(%rbp),%rdx
    18003e07f:	mov    %rax,%rcx
    18003e082:	call   0x18003fbc0
    18003e087:	mov    %rax,%rcx
    18003e08a:	call   0x18003fc30
    18003e08f:	mov    %rax,%r8
    18003e092:	mov    0xacdf(%rip),%r10        # 0x180048d78
@@ -79654,15 +79654,15 @@
    18003e1bf:	call   0x18003f750
    18003e1c4:	test   %al,%al
    18003e1c6:	je     0x18003e56e
    18003e1cc:	nopl   0x0(%rax)
    18003e1d0:	lea    0x60(%rsp),%rcx
    18003e1d5:	call   0x180002a60
    18003e1da:	mov    %rax,%rbx
-   18003e1dd:	lea    0xc900(%rip),%r8        # 0x18004aae4
+   18003e1dd:	lea    0xc908(%rip),%r8        # 0x18004aaec
    18003e1e4:	lea    0xc8(%rbp),%rdx
    18003e1eb:	mov    %rax,%rcx
    18003e1ee:	call   0x18003fbc0
    18003e1f3:	mov    %rax,%rcx
    18003e1f6:	call   0x18003fc30
    18003e1fb:	mov    %rax,%r8
    18003e1fe:	mov    0xab73(%rip),%r10        # 0x180048d78
@@ -79904,15 +79904,15 @@
    18003e5b0:	call   0x18003f750
    18003e5b5:	test   %al,%al
    18003e5b7:	je     0x18003e8e7
    18003e5bd:	nopl   (%rax)
    18003e5c0:	lea    0x60(%rsp),%rcx
    18003e5c5:	call   0x180002a60
    18003e5ca:	mov    %rax,%rbx
-   18003e5cd:	lea    0xc510(%rip),%r8        # 0x18004aae4
+   18003e5cd:	lea    0xc518(%rip),%r8        # 0x18004aaec
    18003e5d4:	lea    0xd8(%rbp),%rdx
    18003e5db:	mov    %rax,%rcx
    18003e5de:	call   0x18003fbc0
    18003e5e3:	mov    %rax,%rcx
    18003e5e6:	call   0x18003fc30
    18003e5eb:	mov    %rax,%r8
    18003e5ee:	mov    0xa783(%rip),%r10        # 0x180048d78
@@ -80127,43 +80127,43 @@
    18003e921:	pop    %r13
    18003e923:	pop    %r12
    18003e925:	pop    %rdi
    18003e926:	pop    %rsi
    18003e927:	pop    %rbx
    18003e928:	pop    %rbp
    18003e929:	ret
-   18003e92a:	lea    0xc197(%rip),%rcx        # 0x18004aac8
+   18003e92a:	lea    0xc19f(%rip),%rcx        # 0x18004aad0
    18003e931:	call   0x1800433b2
    18003e936:	nop
-   18003e937:	lea    0xc18a(%rip),%rcx        # 0x18004aac8
+   18003e937:	lea    0xc192(%rip),%rcx        # 0x18004aad0
    18003e93e:	call   0x1800433b2
    18003e943:	int3
    18003e944:	lea    0xc1c5(%rip),%rdx        # 0x18004ab10
    18003e94b:	lea    0x30(%rbp),%rcx
    18003e94f:	call   0x180004380
    18003e954:	lea    0x158dd(%rip),%rdx        # 0x180054238
    18003e95b:	lea    0x30(%rbp),%rcx
    18003e95f:	call   0x180044848
    18003e964:	nop
    18003e965:	lea    0xb914(%rip),%rcx        # 0x18004a280
    18003e96c:	call   0x1800433b2
    18003e971:	int3
-   18003e972:	lea    0xc14f(%rip),%rcx        # 0x18004aac8
+   18003e972:	lea    0xc157(%rip),%rcx        # 0x18004aad0
    18003e979:	call   0x1800433b2
    18003e97e:	int3
-   18003e97f:	lea    0xc142(%rip),%rcx        # 0x18004aac8
+   18003e97f:	lea    0xc14a(%rip),%rcx        # 0x18004aad0
    18003e986:	call   0x1800433b2
    18003e98b:	int3
    18003e98c:	lea    0xb8ed(%rip),%rcx        # 0x18004a280
    18003e993:	call   0x1800433b2
    18003e998:	int3
-   18003e999:	lea    0xc128(%rip),%rcx        # 0x18004aac8
+   18003e999:	lea    0xc130(%rip),%rcx        # 0x18004aad0
    18003e9a0:	call   0x1800433b2
    18003e9a5:	int3
-   18003e9a6:	lea    0xc11b(%rip),%rcx        # 0x18004aac8
+   18003e9a6:	lea    0xc123(%rip),%rcx        # 0x18004aad0
    18003e9ad:	call   0x1800433b2
    18003e9b2:	int3
    18003e9b3:	int3
    18003e9b4:	int3
    18003e9b5:	int3
    18003e9b6:	int3
    18003e9b7:	int3
@@ -96193,76 +96193,77 @@
    18004aa62:	rex.WB
    18004aa63:	rex.WRXB pop %r12
    18004aa65:	rex.WRXB jo 0x18004aacd
    18004aa68:	outsb  %ds:(%rsi),(%dx)
    18004aa69:	rex.RXB
    18004aa6a:	outsl  %gs:(%rsi),(%dx)
    18004aa6c:	fs gs sub $0x332e3431,%eax
-   18004aa73:	cs xor %ch,0x366e6977(%rip)        # 0x1b67313f1
-   18004aa7a:	xor    $0x5c,%al
-   18004aa7c:	imul   $0x6564756c,0x63(%rsi),%ebp
-   18004aa83:	pop    %rsp
-   18004aa84:	movsxd 0x6c(%rax),%esi
-   18004aa87:	pop    %rdi
-   18004aa88:	movsxd 0x6e(%rdi),%ebp
-   18004aa8b:	jbe    0x18004aabb
-   18004aa8d:	push   $0x20660000
-   18004aa92:	cmp    $0x756e203d,%eax
-   18004aa97:	insb   (%dx),%es:(%rdi)
-   18004aa98:	insb   (%dx),%es:(%rdi)
-   18004aa99:	jo     0x18004ab0f
-   18004aa9b:	jb     0x18004aabd
-   18004aa9d:	jl     0x18004ab1b
-   18004aa9f:	and    %ah,0x6e(%rcx,%rdi,2)
-   18004aaa3:	(bad)
-   18004aaa4:	insl   (%dx),%es:(%rdi)
-   18004aaa5:	imul   $0x74736163,0x5f(%rbx),%esp
-   18004aaac:	cmp    $0x54,%al
-   18004aaae:	outsl  %ds:(%rsi),(%dx)
-   18004aaaf:	ds sub %ah,0x29(%rsi)
-   18004aab3:	and    %ah,(%rcx)
-   18004aab5:	cmp    $0x6c756e20,%eax
-   18004aaba:	insb   (%dx),%es:(%rdi)
-   18004aabb:	jo     0x18004ab31
-   18004aabd:	jb     0x18004aabf
-   18004aabf:	add    %al,(%rax)
-   18004aac1:	add    %al,(%rax)
-   18004aac3:	add    %bh,%bh
-   18004aac5:	(bad)
-   18004aac6:	(bad)
-   18004aac7:	jmp    *0x62(%rcx)
-   18004aaca:	jae    0x18004ab38
-   18004aacc:	cmp    (%rdx),%bh
-   18004aace:	jae    0x18004ab44
-   18004aad0:	jb     0x18004ab3b
-   18004aad2:	outsb  %ds:(%rsi),(%dx)
-   18004aad3:	addr32 pop %rdi
-   18004aad5:	jbe    0x18004ab40
-   18004aad7:	gs ja  0x18004ab14
-   18004aada:	cmp    0x75(%rbx),%dh
-   18004aadd:	(bad)
-   18004aae2:	add    %al,(%rax)
-   18004aae4:	outsb  %ds:(%rsi),(%dx)
+   18004aa73:	cs xor %ch,0x322e6372(%rip)        # 0x1b2330dec
+   18004aa7a:	sub    $0x366e6977,%eax
+   18004aa7f:	xor    $0x5c,%al
+   18004aa81:	imul   $0x6564756c,0x63(%rsi),%ebp
+   18004aa88:	pop    %rsp
+   18004aa89:	movsxd 0x6c(%rax),%esi
+   18004aa8c:	pop    %rdi
+   18004aa8d:	movsxd 0x6e(%rdi),%ebp
+   18004aa90:	jbe    0x18004aac0
+   18004aa92:	push   $0x0
+   18004aa97:	add    %ah,0x20(%rsi)
+   18004aa9a:	cmp    $0x756e203d,%eax
+   18004aa9f:	insb   (%dx),%es:(%rdi)
+   18004aaa0:	insb   (%dx),%es:(%rdi)
+   18004aaa1:	jo     0x18004ab17
+   18004aaa3:	jb     0x18004aac5
+   18004aaa5:	jl     0x18004ab23
+   18004aaa7:	and    %ah,0x6e(%rcx,%rdi,2)
+   18004aaab:	(bad)
+   18004aaac:	insl   (%dx),%es:(%rdi)
+   18004aaad:	imul   $0x74736163,0x5f(%rbx),%esp
+   18004aab4:	cmp    $0x54,%al
+   18004aab6:	outsl  %ds:(%rsi),(%dx)
+   18004aab7:	ds sub %ah,0x29(%rsi)
+   18004aabb:	and    %ah,(%rcx)
+   18004aabd:	cmp    $0x6c756e20,%eax
+   18004aac2:	insb   (%dx),%es:(%rdi)
+   18004aac3:	jo     0x18004ab39
+   18004aac5:	jb     0x18004aac7
+   18004aac7:	add    %al,(%rax)
+   18004aac9:	add    %al,(%rax)
+   18004aacb:	add    %bh,%bh
+   18004aacd:	(bad)
+   18004aace:	(bad)
+   18004aacf:	jmp    *0x62(%rcx)
+   18004aad2:	jae    0x18004ab40
+   18004aad4:	cmp    (%rdx),%bh
+   18004aad6:	jae    0x18004ab4c
+   18004aad8:	jb     0x18004ab43
+   18004aada:	outsb  %ds:(%rsi),(%dx)
+   18004aadb:	addr32 pop %rdi
+   18004aadd:	jbe    0x18004ab48
+   18004aadf:	gs ja  0x18004ab1c
+   18004aae2:	cmp    0x75(%rbx),%dh
    18004aae5:	(bad)
-   18004aae6:	insl   (%dx),%es:(%rdi)
-   18004aae7:	add    %al,%gs:(%rax)
    18004aaea:	add    %al,(%rax)
-   18004aaec:	jne    0x18004ab5c
-   18004aaee:	imul   $0x0,0x0(%rbx,%rsi,2),%esi
-   18004aaf6:	add    %al,(%rax)
-   18004aaf8:	jne    0x18004ab6d
-   18004aafa:	gs pop %rdi
-   18004aafc:	(bad)
-   18004aafe:	jae    0x18004ab65
-   18004ab00:	pop    %rdi
-   18004ab01:	outsb  %ds:(%rsi),(%dx)
-   18004ab02:	(bad)
-   18004ab03:	insl   (%dx),%es:(%rdi)
-   18004ab04:	gs jae 0x18004ab07
-	...
+   18004aaec:	outsb  %ds:(%rsi),(%dx)
+   18004aaed:	(bad)
+   18004aaee:	insl   (%dx),%es:(%rdi)
+   18004aaef:	add    %al,%gs:(%rax)
+   18004aaf2:	add    %al,(%rax)
+   18004aaf4:	jne    0x18004ab64
+   18004aaf6:	imul   $0x0,0x0(%rbx,%rsi,2),%esi
+   18004aafe:	add    %al,(%rax)
+   18004ab00:	jne    0x18004ab75
+   18004ab02:	gs pop %rdi
+   18004ab04:	(bad)
+   18004ab06:	jae    0x18004ab6d
+   18004ab08:	pop    %rdi
+   18004ab09:	outsb  %ds:(%rsi),(%dx)
+   18004ab0a:	(bad)
+   18004ab0b:	insl   (%dx),%es:(%rdi)
+   18004ab0c:	gs jae 0x18004ab0f
    18004ab0f:	add    %bl,0x53(%rbx)
    18004ab12:	push   %rbp
    18004ab13:	push   %rbx
    18004ab14:	je     0x18004ab77
    18004ab16:	movsxd 0x53(%rbx),%ebp
    18004ab19:	rex.WXB push %r13
    18004ab1b:	rex.B
@@ -96923,16 +96924,16 @@
    18004b181:	in     (%dx),%al
    18004b182:	add    $0x180,%eax
    18004b187:	add    %al,%al
    18004b189:	in     (%dx),%al
    18004b18a:	add    $0x180,%eax
    18004b18f:	add    %al,(%rax)
    18004b191:	add    %al,(%rax)
-   18004b193:	add    %cl,0x648127(%rdx)
-   18004b199:	add    %al,(%rax)
+   18004b193:	add    %dl,-0x64(%rdi)
+   18004b196:	andb   $0x0,0x0(%rax,%rax,1)
    18004b19b:	add    %cl,0x50000000(%rip)        # 0x1d004b1a1
    18004b1a1:	add    (%rax),%eax
    18004b1a3:	add    %bl,%ah
    18004b1a5:	flds   (%rax,%rax,1)
    18004b1a8:	fmul   %st,%st(5)
    18004b1aa:	add    $0x0,%al
    18004b1ac:	add    %al,(%rax)
@@ -129015,18 +129016,16 @@
    18005e9d1:	jo     0x18005ea48
    18005e9d3:	je     0x18005ea1e
    18005e9d5:	insl   (%dx),%es:(%rdi)
    18005e9d6:	jo     0x18005ea44
    18005e9d8:	rex.X push %rdx
    18005e9da:	gs jo  0x18005ea1d
    18005e9dd:	(bad)
-   18005e9de:	xor    %dil,0x39(%r8)
-   18005e9e2:	cmp    %ah,0x38(%rsi)
-   18005e9e5:	(bad)
-   18005e9e6:	xor    0x66(%rdx),%ah
+   18005e9de:	xor    %dil,0x35(%r8)
+   18005e9e2:	cmp    %dh,0x35653330(,%rsi,1)
    18005e9e9:	rex
    18005e9ea:	rex add %al,(%rax)
    18005e9ed:	add    %al,(%rax)
    18005e9ef:	add    %dh,-0x4f(%rax)
    18005e9f2:	add    $0x80,%al
    18005e9f4:	add    %eax,(%rax)
 	...
@@ -129064,22 +129063,21 @@
    18005ea49:	jo     0x18005eac0
    18005ea4b:	je     0x18005ea96
    18005ea4d:	insl   (%dx),%es:(%rdi)
    18005ea4e:	jo     0x18005eabc
    18005ea50:	push   %rbx
    18005ea51:	rex.WRB
    18005ea52:	rex (bad)
-   18005ea54:	xor    %dil,0x64(%r8)
-   18005ea58:	(bad)
-   18005ea59:	gs xor $0x35,%al
-   18005ea5c:	gs (bad)
-   18005ea5e:	xor    $0x40,%al
-   18005ea60:	rex add %al,(%rax)
+   18005ea54:	xor    %dil,0x66(%r8)
+   18005ea58:	cmp    %si,(%rax,%rdi,1)
+   18005ea5c:	(bad)
+   18005ea5d:	xor    $0x404030,%eax
 	...
-   18005ea6f:	add    %dh,-0x4f(%rax)
+   18005ea6e:	add    %al,(%rax)
+   18005ea70:	jo     0x18005ea23
    18005ea72:	add    $0x80,%al
    18005ea74:	add    %eax,(%rax)
 	...
    18005ea7e:	add    %al,(%rax)
    18005ea80:	cs (bad)
    18005ea82:	push   %r14
    18005ea84:	(bad)
```

## Comparing `OpenGeode_GeosciencesIO-4.1.4.dist-info/METADATA` & `OpenGeode_GeosciencesIO-4.1.4rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OpenGeode-GeosciencesIO
-Version: 4.1.4
+Version: 4.1.4rc1
 Summary: Input/Output formats for OpenGeode-Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-GeosciencesIO
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.3.0)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.11)
+Requires-Dist: opengeode-core (==14.*,>=14.3.0rc2)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.11rc1)
 
 <h1 align="center">OpenGeode-GeosciencesIO<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Input/Output formats for OpenGeode-Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.1.4 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.1.4rc1 Summary:
 Input/Output formats for OpenGeode-Geosciences Home-page: https://github.com/
 Geode-solutions/OpenGeode-GeosciencesIO Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: MIT Platform: UNKNOWN Description-Content-
-Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.3.0) Requires-
-Dist: opengeode-geosciences (==7.*,>=7.0.11)
+Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.3.0rc2)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.11rc1)
             ****** OpenGeode-GeosciencesIOby Geode-solutions ******
            **** Input/Output formats for OpenGeode-Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-GeosciencesIO provides input and output formats
 for [OpenGeode-Geosciences] objects. [OpenGeode-Geosciences]: https://
```

