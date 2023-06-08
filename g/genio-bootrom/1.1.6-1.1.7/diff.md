# Comparing `tmp/genio_bootrom-1.1.6-py3-none-any.whl.zip` & `tmp/genio_bootrom-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32599 bytes, number of entries: 10
--rw-rw-r--  2.0 unx        0 b- defN 23-May-03 08:15 aiot_bootrom/__init__.py
--rw-rw-r--  2.0 unx      488 b- defN 23-May-03 08:15 aiot_bootrom/bootrom.py
--rwxrwxr-x  2.0 unx    18712 b- defN 23-May-03 08:15 aiot_bootrom/bin/bootrom-tool
--rwxrwxr-x  2.0 unx    29696 b- defN 23-May-03 08:15 aiot_bootrom/bin/bootrom-tool.exe
--rw-rw-r--  2.0 unx    25160 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx      593 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx      102 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      853 b- defN 23-May-03 08:49 genio_bootrom-1.1.6.dist-info/RECORD
-10 files, 75709 bytes uncompressed, 31129 bytes compressed:  58.9%
+Zip file size: 32614 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-08 03:15 aiot_bootrom/__init__.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Jun-08 03:15 aiot_bootrom/bootrom.py
+-rwxr-xr-x  2.0 unx    18712 b- defN 23-Jun-08 03:11 aiot_bootrom/bin/bootrom-tool
+-rwxr-xr-x  2.0 unx    29696 b- defN 23-Jun-08 03:11 aiot_bootrom/bin/bootrom-tool.exe
+-rw-rw-r--  2.0 unx    25160 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      593 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      102 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      853 b- defN 23-Jun-08 03:21 genio_bootrom-1.1.7.dist-info/RECORD
+10 files, 75709 bytes uncompressed, 31144 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: aiot_bootrom/bin/bootrom-tool
 Comment: 
 
 Filename: aiot_bootrom/bin/bootrom-tool.exe
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/LICENSE
+Filename: genio_bootrom-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/METADATA
+Filename: genio_bootrom-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/WHEEL
+Filename: genio_bootrom-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/entry_points.txt
+Filename: genio_bootrom-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/top_level.txt
+Filename: genio_bootrom-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: genio_bootrom-1.1.6.dist-info/RECORD
+Filename: genio_bootrom-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiot_bootrom/bin/bootrom-tool

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --program-header {}

```diff
@@ -6,21 +6,21 @@
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   PHDR           0x000040 0x0000000000000040 0x0000000000000040 0x0002d8 0x0002d8 R   0x8
   INTERP         0x000318 0x0000000000000318 0x0000000000000318 0x00001c 0x00001c R   0x1
       [Requesting program interpreter: /lib64/ld-linux-x86-64.so.2]
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000ff8 0x000ff8 R   0x1000
   LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x001f25 0x001f25 R E 0x1000
-  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x000998 0x000998 R   0x1000
+  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x0009a8 0x0009a8 R   0x1000
   LOAD           0x003c98 0x0000000000004c98 0x0000000000004c98 0x000408 0x000438 RW  0x1000
   DYNAMIC        0x003ca8 0x0000000000004ca8 0x0000000000004ca8 0x000200 0x000200 RW  0x8
   NOTE           0x000338 0x0000000000000338 0x0000000000000338 0x000020 0x000020 R   0x8
   NOTE           0x000358 0x0000000000000358 0x0000000000000358 0x000044 0x000044 R   0x4
   GNU_PROPERTY   0x000338 0x0000000000000338 0x0000000000000338 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x003490 0x0000000000003490 0x0000000000003490 0x0000bc 0x0000bc R   0x4
+  GNU_EH_FRAME   0x0034a0 0x00000000000034a0 0x00000000000034a0 0x0000bc 0x0000bc R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x003c98 0x0000000000004c98 0x0000000000004c98 0x000368 0x000368 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     
    01     .interp
```

### readelf --wide --sections {}

```diff
@@ -16,17 +16,17 @@
   [11] .rela.plt         RELA            0000000000000cb0 000cb0 000348 18  AI  6  24  8
   [12] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [13] .plt              PROGBITS        0000000000001020 001020 000240 10  AX  0   0 16
   [14] .plt.got          PROGBITS        0000000000001260 001260 000010 10  AX  0   0 16
   [15] .plt.sec          PROGBITS        0000000000001270 001270 000230 10  AX  0   0 16
   [16] .text             PROGBITS        00000000000014a0 0014a0 001a75 00  AX  0   0 16
   [17] .fini             PROGBITS        0000000000002f18 002f18 00000d 00  AX  0   0  4
-  [18] .rodata           PROGBITS        0000000000003000 003000 000490 00   A  0   0 16
-  [19] .eh_frame_hdr     PROGBITS        0000000000003490 003490 0000bc 00   A  0   0  4
-  [20] .eh_frame         PROGBITS        0000000000003550 003550 000448 00   A  0   0  8
+  [18] .rodata           PROGBITS        0000000000003000 003000 0004a0 00   A  0   0 16
+  [19] .eh_frame_hdr     PROGBITS        00000000000034a0 0034a0 0000bc 00   A  0   0  4
+  [20] .eh_frame         PROGBITS        0000000000003560 003560 000448 00   A  0   0  8
   [21] .init_array       INIT_ARRAY      0000000000004c98 003c98 000008 08  WA  0   0  8
   [22] .fini_array       FINI_ARRAY      0000000000004ca0 003ca0 000008 08  WA  0   0  8
   [23] .dynamic          DYNAMIC         0000000000004ca8 003ca8 000200 10  WA  7   0  8
   [24] .got              PROGBITS        0000000000004ea8 003ea8 000158 08  WA  0   0  8
   [25] .data             PROGBITS        0000000000005000 004000 0000a0 00  WA  0   0 32
   [26] .bss              NOBITS          00000000000050a0 0040a0 000030 00  WA  0   0 32
   [27] .comment          PROGBITS        0000000000000000 0040a0 00002b 01  MS  0   0  1
```

### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ee7e20b7be1b13fb7058b743e3d2ab66fa8a203a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a8a82421ba9aebe5dc0ffcbc4c17e77b03a00759
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

### strings --all --bytes=8 {}

```diff
@@ -58,20 +58,20 @@
 bootstrap-mode
 Failed to load bootstrap %s: %d
 Failed to load bootstrap sign %s: %d
 Failed to connect to bootrom: %d
 Failed to jump to bootstrap: %d
 Sending auth to address: %#x
 	-> Invalid checksum
-Opening %s using baudate=%u
+Opening %s using baudrate=%u
 Sending bootstrap to address: %#x
 Jumping to bootstrap at address %#x in AArch32 mode
 Jumping to bootstrap at address %#x in AArch64 mode
 Looking for MediaTek SoC matching USB device %.4x:%.4x
-Connected to MediaTek MT%.4x SoC
+Connected to MediaTek SoC: hw_code[0x%.4x]
 Failed to create udev handle
 usb_device
 idVendor
 idProduct
 Failed to create udev enumerate
 Failed to get udev device list
 write(): %s
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -804,15 +804,15 @@
 	mov    %rax,0x120(%rsp)
 	movl   $0x3,0x128(%rsp)
 	movl   $0x4,0x148(%rsp)
 	mov    %rcx,0x10(%rsp)
 	jne    2510 <usleep@plt+0x1080>
 	mov    %esi,%edx
 	mov    $0x1,%edi
-	lea    0x10a1(%rip),%rsi        
+	lea    0x10a9(%rip),%rsi        
 	xor    %eax,%eax
 	mov    %r9,%r13
 	lea    0x150(%rsp),%r14
 	lea    0x1029(%rip),%rbp        
 	call   13c0 <__printf_chk@plt>
 	cmpl   $0x4,0x18(%r15)
 	ja     223e <usleep@plt+0xdae>
@@ -1049,15 +1049,15 @@
 	mov    %fs:0x28,%rax
 	mov    %rax,0x68(%rsp)
 	xor    %eax,%eax
 	mov    %rsp,%rdi
 	rep stos %rax,%es:(%rdi)
 	mov    %esi,0x28(%rsp)
 	mov    $0x1,%edi
-	lea    0xd27(%rip),%rsi        
+	lea    0xd2f(%rip),%rsi        
 	movl   $0xd5,0x8(%rsp)
 	movl   $0x1,0x38(%rsp)
 	movl   $0x4,0x58(%rsp)
 	call   13c0 <__printf_chk@plt>
 	mov    %rsp,%rsi
 	mov    %rbp,%rdi
 	call   1aa0 <usleep@plt+0x610>
@@ -1078,15 +1078,15 @@
 	mov    %fs:0x28,%rax
 	mov    %rax,0xc8(%rsp)
 	xor    %eax,%eax
 	mov    %rsp,%rdi
 	rep stos %rax,%es:(%rdi)
 	mov    %esi,0x28(%rsp)
 	mov    $0x1,%edi
-	lea    0xcd9(%rip),%rsi        
+	lea    0xce1(%rip),%rsi        
 	movl   $0xde,0x8(%rsp)
 	movl   $0x1,0x38(%rsp)
 	movl   $0x1,0x48(%rsp)
 	movl   $0x4,0x78(%rsp)
 	movl   $0x64,0x88(%rsp)
 	movl   $0x4,0xb8(%rsp)
 	call   13c0 <__printf_chk@plt>
@@ -1106,15 +1106,15 @@
 	mov    $0x3,%ecx
 	mov    $0xe8d,%edx
 	push   %r13
 	mov    %rdi,%r13
 	mov    $0x1,%edi
 	push   %r12
 	mov    %esi,%r12d
-	lea    0xc7a(%rip),%rsi        
+	lea    0xc82(%rip),%rsi        
 	push   %rbp
 	push   %rbx
 	sub    $0xf0,%rsp
 	mov    %fs:0x28,%rax
 	mov    %rax,0xe8(%rsp)
 	xor    %eax,%eax
 	lea    0x80(%rsp),%rbp
@@ -1183,15 +1183,15 @@
 	movl   $0x3,0x48(%rsp)
 	movl   $0x4,0x68(%rsp)
 	call   1aa0 <usleep@plt+0x610>
 	mov    %eax,%r12d
 	test   %eax,%eax
 	jne    2721 <usleep@plt+0x1291>
 	movzwl 0xe(%rsp),%edx
-	lea    0xb67(%rip),%rsi        
+	lea    0xb6f(%rip),%rsi        
 	mov    $0x1,%edi
 	xor    %eax,%eax
 	call   13c0 <__printf_chk@plt>
 	jmp    2721 <usleep@plt+0x1291>
 	mov    $0xfffffffb,%r12d
 	jmp    2721 <usleep@plt+0x1291>
 	call   1300 <__stack_chk_fail@plt>
@@ -1213,44 +1213,44 @@
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   1350 <udev_enumerate_new@plt>
 	mov    %rax,0x18(%rsp)
 	test   %rax,%rax
 	je     29d9 <usleep@plt+0x1549>
 	mov    %rax,%rbx
-	lea    0xb2b(%rip),%rsi        
+	lea    0xb3d(%rip),%rsi        
 	mov    %rax,%rdi
 	call   12f0 <udev_enumerate_add_match_subsystem@plt>
 	mov    %rbx,%rdi
 	call   1290 <udev_enumerate_scan_devices@plt>
 	mov    %rbx,%rdi
 	call   1370 <udev_enumerate_get_list_entry@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
 	je     2a01 <usleep@plt+0x1571>
-	lea    0xb04(%rip),%rbx        
+	lea    0xb16(%rip),%rbx        
 	nopl   0x0(%rax,%rax,1)
 	mov    %rbp,%rdi
 	call   13e0 <udev_list_entry_get_name@plt>
 	mov    %r12,%rdi
 	mov    %rax,%rsi
 	call   1320 <udev_device_new_from_syspath@plt>
 	mov    %rbx,%rdx
-	lea    0xaea(%rip),%rsi        
+	lea    0xafc(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r14
 	call   1360 <udev_device_get_parent_with_subsystem_devtype@plt>
 	mov    %rax,%r15
 	test   %rax,%rax
 	je     2990 <usleep@plt+0x1500>
-	lea    0xad0(%rip),%rsi        
+	lea    0xae2(%rip),%rsi        
 	mov    %rax,%rdi
 	call   13b0 <udev_device_get_sysattr_value@plt>
 	mov    %r15,%rdi
-	lea    0xac7(%rip),%rsi        
+	lea    0xad9(%rip),%rsi        
 	mov    %rax,%r13
 	call   13b0 <udev_device_get_sysattr_value@plt>
 	mov    %rax,%r15
 	test   %r13,%r13
 	je     2990 <usleep@plt+0x1500>
 	test   %rax,%rax
 	je     2990 <usleep@plt+0x1500>
@@ -1264,15 +1264,15 @@
 	mov    %rax,%r13
 	call   1380 <strtol@plt>
 	cmp    $0xe8d,%r13
 	jne    2990 <usleep@plt+0x1500>
 	cmp    $0x3,%rax
 	jne    2990 <usleep@plt+0x1500>
 	mov    %r14,%rdi
-	lea    0xa7a(%rip),%rsi        
+	lea    0xa8c(%rip),%rsi        
 	call   1440 <udev_device_get_property_value@plt>
 	mov    0x10(%rsp),%rdx
 	mov    0x8(%rsp),%rdi
 	mov    %rax,%rsi
 	call   1280 <strncpy@plt>
 	mov    %r14,%rdi
 	xor    %r14d,%r14d
@@ -1299,29 +1299,29 @@
 	test   %rax,%rax
 	jne    28a0 <usleep@plt+0x1410>
 	mov    $0xffffffed,%r14d
 	jmp    2966 <usleep@plt+0x14d6>
 	mov    $0x1d,%edx
 	mov    0x2700(%rip),%rcx        
 	mov    $0x1,%esi
-	lea    0x9ae(%rip),%rdi        
+	lea    0x9c0(%rip),%rdi        
 	mov    $0xfffffffb,%r14d
 	call   1460 <fwrite@plt>
 	jmp    2978 <usleep@plt+0x14e8>
 	mov    $0x20,%edx
 	mov    0x26db(%rip),%rcx        
 	mov    $0x1,%esi
-	lea    0x9d7(%rip),%rdi        
+	lea    0x9e7(%rip),%rdi        
 	mov    $0xfffffffb,%r14d
 	call   1460 <fwrite@plt>
 	jmp    2978 <usleep@plt+0x14e8>
 	mov    $0x1f,%edx
 	mov    0x26b3(%rip),%rcx        
 	mov    $0x1,%esi
-	lea    0x9d7(%rip),%rdi        
+	lea    0x9e7(%rip),%rdi        
 	mov    $0xfffffffb,%r14d
 	call   1460 <fwrite@plt>
 	jmp    2978 <usleep@plt+0x14e8>
 	nopl   0x0(%rax)
 	endbr64
 	push   %rbp
 	mov    $0x1,%edx
@@ -1349,15 +1349,15 @@
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
-	lea    0x97a(%rip),%rdx        
+	lea    0x98a(%rip),%rdx        
 	mov    %rax,%rcx
 	mov    0x2620(%rip),%rdi        
 	mov    $0x1,%esi
 	xor    %eax,%eax
 	call   1470 <__fprintf_chk@plt>
 	mov    (%rbx),%eax
 	add    $0x8,%rsp
@@ -1366,15 +1366,15 @@
 	neg    %eax
 	ret
 	nopw   0x0(%rax,%rax,1)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
-	lea    0x947(%rip),%rdx        
+	lea    0x957(%rip),%rdx        
 	mov    %rax,%rcx
 	jmp    2a99 <usleep@plt+0x1609>
 	nopl   0x0(%rax,%rax,1)
 	mov    $0xfffffffb,%eax
 	jmp    2a75 <usleep@plt+0x15e5>
 	nopw   0x0(%rax,%rax,1)
 	endbr64
@@ -1420,29 +1420,29 @@
 	pop    %r12
 	ret
 	nopl   0x0(%rax)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
-	lea    0x87a(%rip),%rdx        
+	lea    0x88a(%rip),%rdx        
 	mov    %rax,%rcx
 	mov    0x2520(%rip),%rdi        
 	mov    $0x1,%esi
 	xor    %eax,%eax
 	call   1470 <__fprintf_chk@plt>
 	mov    (%rbx),%eax
 	neg    %eax
 	jmp    2b60 <usleep@plt+0x16d0>
 	nopw   0x0(%rax,%rax,1)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
-	lea    0x84f(%rip),%rdx        
+	lea    0x85f(%rip),%rdx        
 	mov    %rax,%rcx
 	jmp    2b99 <usleep@plt+0x1709>
 	nopl   0x0(%rax,%rax,1)
 	mov    $0xfffffffb,%eax
 	jmp    2b60 <usleep@plt+0x16d0>
 	call   1300 <__stack_chk_fail@plt>
 	data16 cs nopw 0x0(%rax,%rax,1)
@@ -1464,15 +1464,15 @@
 	cs nopw 0x0(%rax,%rax,1)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    0x248a(%rip),%rdi        
 	mov    $0x1,%esi
-	lea    0x7db(%rip),%rdx        
+	lea    0x7eb(%rip),%rdx        
 	mov    %rax,%rcx
 	xor    %eax,%eax
 	call   1470 <__fprintf_chk@plt>
 	mov    (%rbx),%eax
 	pop    %rbx
 	neg    %eax
 	ret
@@ -1498,15 +1498,15 @@
 	nopl   (%rax)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    0x2422(%rip),%rdi        
 	mov    $0x1,%esi
-	lea    0x766(%rip),%rdx        
+	lea    0x776(%rip),%rdx        
 	mov    %rax,%rcx
 	xor    %eax,%eax
 	call   1470 <__fprintf_chk@plt>
 	mov    (%rbx),%eax
 	pop    %rbx
 	neg    %eax
 	ret
@@ -1547,15 +1547,15 @@
 	je     2de0 <usleep@plt+0x1950>
 	mov    %rsp,%r14
 	mov    %eax,%edi
 	mov    %r14,%rsi
 	call   13f0 <tcgetattr@plt>
 	cmp    $0xffffffff,%eax
 	je     2e30 <usleep@plt+0x19a0>
-	movdqa 0x724(%rip),%xmm0        
+	movdqa 0x734(%rip),%xmm0        
 	mov    $0x100,%eax
 	mov    $0x1002,%esi
 	mov    %r14,%rdi
 	mov    %ax,0x16(%rsp)
 	movaps %xmm0,(%rsp)
 	call   1430 <cfsetispeed@plt>
 	cmp    $0xffffffff,%eax
@@ -1598,42 +1598,42 @@
 	jmp    2db6 <usleep@plt+0x1926>
 	nopl   (%rax)
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    %r13,%rcx
-	lea    0x613(%rip),%rdx        
+	lea    0x623(%rip),%rdx        
 	mov    %rax,%r8
 	jmp    2df4 <usleep@plt+0x1964>
 	xchg   %ax,%ax
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    %r13,%rcx
-	lea    0x5e0(%rip),%rdx        
+	lea    0x5f0(%rip),%rdx        
 	mov    %rax,%r8
 	jmp    2df4 <usleep@plt+0x1964>
 	xchg   %ax,%ax
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    %r13,%rcx
-	lea    0x5e8(%rip),%rdx        
+	lea    0x5f8(%rip),%rdx        
 	mov    %rax,%r8
 	jmp    2df4 <usleep@plt+0x1964>
 	xchg   %ax,%ax
 	call   1270 <__errno_location@plt>
 	mov    (%rax),%edi
 	mov    %rax,%rbx
 	call   1480 <strerror@plt>
 	mov    %r13,%rcx
-	lea    0x5dd(%rip),%rdx        
+	lea    0x5ed(%rip),%rdx        
 	mov    %rax,%r8
 	jmp    2df4 <usleep@plt+0x1964>
 	mov    $0xffffffea,%eax
 	jmp    2db6 <usleep@plt+0x1926>
 	call   1300 <__stack_chk_fail@plt>
 	endbr64
 	push   %r15
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -36,41 +36,42 @@
   0x00003210 58ecffff f0ebffff d0ebffff a8ebffff X...............
   0x00003220 30ecffff a4f2ffff 34f2ffff 14f2ffff 0.......4.......
   0x00003230 fcefffff 7cf2ffff 53656e64 696e6720 ....|...Sending 
   0x00003240 61757468 20746f20 61646472 6573733a auth to address:
   0x00003250 20252378 0a00092d 3e20496e 76616c69  %#x...-> Invali
   0x00003260 64206368 65636b73 756d004f 70656e69 d checksum.Openi
   0x00003270 6e672025 73207573 696e6720 62617564 ng %s using baud
-  0x00003280 6174653d 25750a00 53656e64 696e6720 ate=%u..Sending 
-  0x00003290 626f6f74 73747261 7020746f 20616464 bootstrap to add
-  0x000032a0 72657373 3a202523 780a0000 00000000 ress: %#x.......
-  0x000032b0 4a756d70 696e6720 746f2062 6f6f7473 Jumping to boots
-  0x000032c0 74726170 20617420 61646472 65737320 trap at address 
-  0x000032d0 25237820 696e2041 41726368 3332206d %#x in AArch32 m
-  0x000032e0 6f64650a 00000000 4a756d70 696e6720 ode.....Jumping 
-  0x000032f0 746f2062 6f6f7473 74726170 20617420 to bootstrap at 
-  0x00003300 61646472 65737320 25237820 696e2041 address %#x in A
-  0x00003310 41726368 3634206d 6f64650a 00000000 Arch64 mode.....
-  0x00003320 4c6f6f6b 696e6720 666f7220 4d656469 Looking for Medi
-  0x00003330 6154656b 20536f43 206d6174 6368696e aTek SoC matchin
-  0x00003340 67205553 42206465 76696365 20252e34 g USB device %.4
-  0x00003350 783a252e 34780a00 436f6e6e 65637465 x:%.4x..Connecte
-  0x00003360 6420746f 204d6564 69615465 6b204d54 d to MediaTek MT
-  0x00003370 252e3478 20536f43 0a004661 696c6564 %.4x SoC..Failed
-  0x00003380 20746f20 63726561 74652075 64657620  to create udev 
-  0x00003390 68616e64 6c650a00 74747900 7573625f handle..tty.usb_
-  0x000033a0 64657669 63650075 73620069 6456656e device.usb.idVen
-  0x000033b0 646f7200 69645072 6f647563 74004445 dor.idProduct.DE
-  0x000033c0 564e414d 45000000 4661696c 65642074 VNAME...Failed t
-  0x000033d0 6f206372 65617465 20756465 7620656e o create udev en
-  0x000033e0 756d6572 6174650a 00000000 00000000 umerate.........
-  0x000033f0 4661696c 65642074 6f206765 74207564 Failed to get ud
-  0x00003400 65762064 65766963 65206c69 73740a00 ev device list..
-  0x00003410 77726974 6528293a 2025730a 00726561 write(): %s..rea
-  0x00003420 6428293a 2025730a 00746367 65746174 d(): %s..tcgetat
-  0x00003430 74722825 73293a20 25730a00 63667365 tr(%s): %s..cfse
-  0x00003440 74697370 65656428 2573293a 2025730a tispeed(%s): %s.
-  0x00003450 00636673 65746f73 70656564 28257329 .cfsetospeed(%s)
-  0x00003460 3a202573 0a007463 73657461 74747228 : %s..tcsetattr(
-  0x00003470 2573293a 2025730a 00000000 00000000 %s): %s.........
-  0x00003480 00000000 00000000 300c0000 00000000 ........0.......
+  0x00003280 72617465 3d25750a 00000000 00000000 rate=%u.........
+  0x00003290 53656e64 696e6720 626f6f74 73747261 Sending bootstra
+  0x000032a0 7020746f 20616464 72657373 3a202523 p to address: %#
+  0x000032b0 780a0000 00000000 4a756d70 696e6720 x.......Jumping 
+  0x000032c0 746f2062 6f6f7473 74726170 20617420 to bootstrap at 
+  0x000032d0 61646472 65737320 25237820 696e2041 address %#x in A
+  0x000032e0 41726368 3332206d 6f64650a 00000000 Arch32 mode.....
+  0x000032f0 4a756d70 696e6720 746f2062 6f6f7473 Jumping to boots
+  0x00003300 74726170 20617420 61646472 65737320 trap at address 
+  0x00003310 25237820 696e2041 41726368 3634206d %#x in AArch64 m
+  0x00003320 6f64650a 00000000 4c6f6f6b 696e6720 ode.....Looking 
+  0x00003330 666f7220 4d656469 6154656b 20536f43 for MediaTek SoC
+  0x00003340 206d6174 6368696e 67205553 42206465  matching USB de
+  0x00003350 76696365 20252e34 783a252e 34780a00 vice %.4x:%.4x..
+  0x00003360 436f6e6e 65637465 6420746f 204d6564 Connected to Med
+  0x00003370 69615465 6b20536f 433a2068 775f636f iaTek SoC: hw_co
+  0x00003380 64655b30 78252e34 785d0a00 4661696c de[0x%.4x]..Fail
+  0x00003390 65642074 6f206372 65617465 20756465 ed to create ude
+  0x000033a0 76206861 6e646c65 0a007474 79007573 v handle..tty.us
+  0x000033b0 625f6465 76696365 00757362 00696456 b_device.usb.idV
+  0x000033c0 656e646f 72006964 50726f64 75637400 endor.idProduct.
+  0x000033d0 4445564e 414d4500 4661696c 65642074 DEVNAME.Failed t
+  0x000033e0 6f206372 65617465 20756465 7620656e o create udev en
+  0x000033f0 756d6572 6174650a 00000000 00000000 umerate.........
+  0x00003400 4661696c 65642074 6f206765 74207564 Failed to get ud
+  0x00003410 65762064 65766963 65206c69 73740a00 ev device list..
+  0x00003420 77726974 6528293a 2025730a 00726561 write(): %s..rea
+  0x00003430 6428293a 2025730a 00746367 65746174 d(): %s..tcgetat
+  0x00003440 74722825 73293a20 25730a00 63667365 tr(%s): %s..cfse
+  0x00003450 74697370 65656428 2573293a 2025730a tispeed(%s): %s.
+  0x00003460 00636673 65746f73 70656564 28257329 .cfsetospeed(%s)
+  0x00003470 3a202573 0a007463 73657461 74747228 : %s..tcsetattr(
+  0x00003480 2573293a 2025730a 00000000 00000000 %s): %s.........
+  0x00003490 00000000 00000000 300c0000 00000000 ........0.......
```

### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,15 +1,15 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00003490 011b033b bc000000 16000000 90dbffff ...;............
-  0x000034a0 f0000000 d0ddffff 18010000 e0ddffff ................
-  0x000034b0 30010000 10e0ffff 7c010000 d0e3ffff 0.......|.......
-  0x000034c0 d8000000 c0e4ffff 48010000 10e6ffff ........H.......
-  0x000034d0 d0010000 e0e8ffff fc010000 30eaffff ............0...
-  0x000034e0 38020000 40eaffff 4c020000 40ecffff 8...@...L...@...
-  0x000034f0 84020000 c0f0ffff d4020000 40f1ffff ............@...
-  0x00003500 f8020000 f0f1ffff 1c030000 90f3ffff ................
-  0x00003510 60030000 a0f5ffff b0030000 60f6ffff `...........`...
-  0x00003520 e8030000 60f7ffff 1c040000 d0f7ffff ....`...........
-  0x00003530 44040000 30f8ffff 64040000 10faffff D...0...d.......
-  0x00003540 a8040000 80faffff f0040000          ............
+  0x000034a0 011b033b bc000000 16000000 80dbffff ...;............
+  0x000034b0 f0000000 c0ddffff 18010000 d0ddffff ................
+  0x000034c0 30010000 00e0ffff 7c010000 c0e3ffff 0.......|.......
+  0x000034d0 d8000000 b0e4ffff 48010000 00e6ffff ........H.......
+  0x000034e0 d0010000 d0e8ffff fc010000 20eaffff ............ ...
+  0x000034f0 38020000 30eaffff 4c020000 30ecffff 8...0...L...0...
+  0x00003500 84020000 b0f0ffff d4020000 30f1ffff ............0...
+  0x00003510 f8020000 e0f1ffff 1c030000 80f3ffff ................
+  0x00003520 60030000 90f5ffff b0030000 50f6ffff `...........P...
+  0x00003530 e8030000 50f7ffff 1c040000 c0f7ffff ....P...........
+  0x00003540 44040000 20f8ffff 64040000 00faffff D... ...d.......
+  0x00003550 a8040000 70faffff f0040000          ....p.......
```

### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,72 +1,72 @@
 
 Hex dump of section '.eh_frame':
-  0x00003550 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00003560 1b0c0708 90010000 14000000 1c000000 ................
-  0x00003570 f0e2ffff 2f000000 00440710 00000000 ..../....D......
-  0x00003580 24000000 34000000 98daffff 40020000 $...4.......@...
-  0x00003590 000e1046 0e184a0f 0b770880 003f1a3a ...F..J..w...?.:
-  0x000035a0 2a332422 00000000 14000000 5c000000 *3$"........\...
-  0x000035b0 b0dcffff 10000000 00000000 00000000 ................
-  0x000035c0 14000000 74000000 a8dcffff 30020000 ....t.......0...
-  0x000035d0 00000000 00000000 30000000 8c000000 ........0.......
-  0x000035e0 70e3ffff 42010000 00420e10 8c02440e p...B....B....D.
-  0x000035f0 1886034c 0e208304 4a0ec001 02970a0e ...L. ..J.......
-  0x00003600 20410e18 410e1042 0e08410b 50000000  A..A..B..A.P...
-  0x00003610 c0000000 8cdeffff bd030000 00460e10 .............F..
-  0x00003620 8f02490e 188e0348 0e208d04 420e288c ..I....H. ..B.(.
-  0x00003630 05440e30 8606440e 3883074b 0ea00103 .D.0..D.8..K....
-  0x00003640 bb020a0e 38440e30 410e2842 0e20420e ....8D.0A.(B. B.
-  0x00003650 18420e10 420e0841 0b000000 00000000 .B..B..A........
-  0x00003660 28000000 14010000 38e4ffff cf020000 (.......8.......
-  0x00003670 00410e10 8602440e 18830347 0e3002c3 .A....D....G.0..
-  0x00003680 0a0e1841 0e10410e 08410b00 38000000 ...A..A..A..8...
-  0x00003690 40010000 dce6ffff 46010000 00420e10 @.......F....B..
-  0x000036a0 8d02490e 188c0344 0e208604 480e2883 ..I....D. ..H.(.
-  0x000036b0 05470e40 02a60a0e 28410e20 410e1842 .G.@....(A. A..B
-  0x000036c0 0e10420e 08460b00 10000000 7c010000 ..B..F......|...
-  0x000036d0 f0e7ffff 0e000000 00000000 34000000 ............4...
-  0x000036e0 90010000 ece7ffff f7010000 00460e10 .............F..
-  0x000036f0 8c02440e 18860344 0e208304 4f0e8002 ..D....D. ..O...
-  0x00003700 03a9010a 0e20410e 18410e10 420e0846 ..... A..A..B..F
-  0x00003710 0b000000 4c000000 c8010000 b4e9ffff ....L...........
-  0x00003720 80040000 00460e10 8f02450e 188e0342 .....F....E....B
-  0x00003730 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
-  0x00003740 3883074a 0ea00303 a9030a0e 38410e30 8..J........8A.0
-  0x00003750 410e2842 0e20420e 18420e10 420e0842 A.(B. B..B..B..B
-  0x00003760 0b000000 20000000 18020000 e4edffff .... ...........
-  0x00003770 7c000000 00450e10 86024e0e 80010262 |....E....N....b
-  0x00003780 0a0e1041 0e08410b 20000000 3c020000 ...A..A. ...<...
-  0x00003790 40eeffff a6000000 00450e10 8602510e @........E....Q.
-  0x000037a0 e0010289 0a0e1041 0e08410b 40000000 .......A..A.@...
-  0x000037b0 60020000 cceeffff 92010000 00460e10 `............F..
-  0x000037c0 8e024c0e 188d034a 0e208c04 4b0e2886 ..L....J. ..K.(.
-  0x000037d0 05410e30 8306470e a0020290 0a0e3044 .A.0..G.......0D
-  0x000037e0 0e28410e 20420e18 420e1042 0e08460b .(A. B..B..B..F.
-  0x000037f0 4c000000 a4020000 28f0ffff 09020000 L.......(.......
-  0x00003800 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
-  0x00003810 420e288c 05410e30 8606410e 38830744 B.(..A.0..A.8..D
-  0x00003820 0e60034a 010a0e38 440e3041 0e28420e .`.J...8D.0A.(B.
-  0x00003830 20420e18 420e1042 0e08470b 00000000  B..B..B..G.....
-  0x00003840 34000000 f4020000 e8f1ffff b7000000 4...............
-  0x00003850 00450e10 8602490e 18830347 0e20740a .E....I....G. t.
-  0x00003860 0e18410e 10410e08 450b720a 0e18410e ..A..A..E.r...A.
-  0x00003870 10410e08 4c0b0000 30000000 2c030000 .A..L...0...,...
-  0x00003880 70f2ffff f4000000 00460e10 8c02460e p........F....F.
-  0x00003890 18860344 0e208304 470e3002 6d0a0e20 ...D. ..G.0.m.. 
-  0x000038a0 410e1841 0e10420e 08480b00 24000000 A..A..B..H..$...
-  0x000038b0 60030000 3cf3ffff 6f000000 00450e10 `...<...o....E..
-  0x000038c0 8302600a 0e084b0b 6f0a0e08 490b460e ..`...K.o...I.F.
-  0x000038d0 08000000 1c000000 88030000 84f3ffff ................
-  0x000038e0 5a000000 00450e10 8302550a 0e084e0b Z....E....U...N.
-  0x000038f0 6f0e0800 40000000 a8030000 c4f3ffff o...@...........
-  0x00003900 e0010000 00460e10 8e02420e 188d0342 .....F....B....B
-  0x00003910 0e208c04 410e2886 05410e30 8306440e . ..A.(..A.0..D.
-  0x00003920 800102fe 0a0e3041 0e28410e 20420e18 ......0A.(A. B..
-  0x00003930 420e1042 0e084a0b 44000000 ec030000 B..B..J.D.......
-  0x00003940 60f5ffff 65000000 00460e10 8f02490e `...e....F....I.
-  0x00003950 188e0345 0e208d04 450e288c 05440e30 ...E. ..E.(..D.0
-  0x00003960 8606480e 38830747 0e406e0e 38410e30 ..H.8..G.@n.8A.0
-  0x00003970 410e2842 0e20420e 18420e10 420e0800 A.(B. B..B..B...
-  0x00003980 10000000 34040000 88f5ffff 05000000 ....4...........
-  0x00003990 00000000 00000000                   ........
+  0x00003560 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00003570 1b0c0708 90010000 14000000 1c000000 ................
+  0x00003580 e0e2ffff 2f000000 00440710 00000000 ..../....D......
+  0x00003590 24000000 34000000 88daffff 40020000 $...4.......@...
+  0x000035a0 000e1046 0e184a0f 0b770880 003f1a3a ...F..J..w...?.:
+  0x000035b0 2a332422 00000000 14000000 5c000000 *3$"........\...
+  0x000035c0 a0dcffff 10000000 00000000 00000000 ................
+  0x000035d0 14000000 74000000 98dcffff 30020000 ....t.......0...
+  0x000035e0 00000000 00000000 30000000 8c000000 ........0.......
+  0x000035f0 60e3ffff 42010000 00420e10 8c02440e `...B....B....D.
+  0x00003600 1886034c 0e208304 4a0ec001 02970a0e ...L. ..J.......
+  0x00003610 20410e18 410e1042 0e08410b 50000000  A..A..B..A.P...
+  0x00003620 c0000000 7cdeffff bd030000 00460e10 ....|........F..
+  0x00003630 8f02490e 188e0348 0e208d04 420e288c ..I....H. ..B.(.
+  0x00003640 05440e30 8606440e 3883074b 0ea00103 .D.0..D.8..K....
+  0x00003650 bb020a0e 38440e30 410e2842 0e20420e ....8D.0A.(B. B.
+  0x00003660 18420e10 420e0841 0b000000 00000000 .B..B..A........
+  0x00003670 28000000 14010000 28e4ffff cf020000 (.......(.......
+  0x00003680 00410e10 8602440e 18830347 0e3002c3 .A....D....G.0..
+  0x00003690 0a0e1841 0e10410e 08410b00 38000000 ...A..A..A..8...
+  0x000036a0 40010000 cce6ffff 46010000 00420e10 @.......F....B..
+  0x000036b0 8d02490e 188c0344 0e208604 480e2883 ..I....D. ..H.(.
+  0x000036c0 05470e40 02a60a0e 28410e20 410e1842 .G.@....(A. A..B
+  0x000036d0 0e10420e 08460b00 10000000 7c010000 ..B..F......|...
+  0x000036e0 e0e7ffff 0e000000 00000000 34000000 ............4...
+  0x000036f0 90010000 dce7ffff f7010000 00460e10 .............F..
+  0x00003700 8c02440e 18860344 0e208304 4f0e8002 ..D....D. ..O...
+  0x00003710 03a9010a 0e20410e 18410e10 420e0846 ..... A..A..B..F
+  0x00003720 0b000000 4c000000 c8010000 a4e9ffff ....L...........
+  0x00003730 80040000 00460e10 8f02450e 188e0342 .....F....E....B
+  0x00003740 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x00003750 3883074a 0ea00303 a9030a0e 38410e30 8..J........8A.0
+  0x00003760 410e2842 0e20420e 18420e10 420e0842 A.(B. B..B..B..B
+  0x00003770 0b000000 20000000 18020000 d4edffff .... ...........
+  0x00003780 7c000000 00450e10 86024e0e 80010262 |....E....N....b
+  0x00003790 0a0e1041 0e08410b 20000000 3c020000 ...A..A. ...<...
+  0x000037a0 30eeffff a6000000 00450e10 8602510e 0........E....Q.
+  0x000037b0 e0010289 0a0e1041 0e08410b 40000000 .......A..A.@...
+  0x000037c0 60020000 bceeffff 92010000 00460e10 `............F..
+  0x000037d0 8e024c0e 188d034a 0e208c04 4b0e2886 ..L....J. ..K.(.
+  0x000037e0 05410e30 8306470e a0020290 0a0e3044 .A.0..G.......0D
+  0x000037f0 0e28410e 20420e18 420e1042 0e08460b .(A. B..B..B..F.
+  0x00003800 4c000000 a4020000 18f0ffff 09020000 L...............
+  0x00003810 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
+  0x00003820 420e288c 05410e30 8606410e 38830744 B.(..A.0..A.8..D
+  0x00003830 0e60034a 010a0e38 440e3041 0e28420e .`.J...8D.0A.(B.
+  0x00003840 20420e18 420e1042 0e08470b 00000000  B..B..B..G.....
+  0x00003850 34000000 f4020000 d8f1ffff b7000000 4...............
+  0x00003860 00450e10 8602490e 18830347 0e20740a .E....I....G. t.
+  0x00003870 0e18410e 10410e08 450b720a 0e18410e ..A..A..E.r...A.
+  0x00003880 10410e08 4c0b0000 30000000 2c030000 .A..L...0...,...
+  0x00003890 60f2ffff f4000000 00460e10 8c02460e `........F....F.
+  0x000038a0 18860344 0e208304 470e3002 6d0a0e20 ...D. ..G.0.m.. 
+  0x000038b0 410e1841 0e10420e 08480b00 24000000 A..A..B..H..$...
+  0x000038c0 60030000 2cf3ffff 6f000000 00450e10 `...,...o....E..
+  0x000038d0 8302600a 0e084b0b 6f0a0e08 490b460e ..`...K.o...I.F.
+  0x000038e0 08000000 1c000000 88030000 74f3ffff ............t...
+  0x000038f0 5a000000 00450e10 8302550a 0e084e0b Z....E....U...N.
+  0x00003900 6f0e0800 40000000 a8030000 b4f3ffff o...@...........
+  0x00003910 e0010000 00460e10 8e02420e 188d0342 .....F....B....B
+  0x00003920 0e208c04 410e2886 05410e30 8306440e . ..A.(..A.0..D.
+  0x00003930 800102fe 0a0e3041 0e28410e 20420e18 ......0A.(A. B..
+  0x00003940 420e1042 0e084a0b 44000000 ec030000 B..B..J.D.......
+  0x00003950 50f5ffff 65000000 00460e10 8f02490e P...e....F....I.
+  0x00003960 188e0345 0e208d04 450e288c 05440e30 ...E. ..E.(..D.0
+  0x00003970 8606480e 38830747 0e406e0e 38410e30 ..H.8..G.@n.8A.0
+  0x00003980 410e2842 0e20420e 18420e10 420e0800 A.(B. B..B..B...
+  0x00003990 10000000 34040000 78f5ffff 05000000 ....4...x.......
+  0x000039a0 00000000 00000000                   ........
```

## aiot_bootrom/bin/bootrom-tool.exe

### objdump

```diff
@@ -28,15 +28,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		0000e000
 SizeOfHeaders		00000400
-CheckSum		0000d899
+CheckSum		00016842
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -2030,15 +2030,15 @@
   40240c:	jne    0x4023e8
   40240e:	mov    0x8f33(%rip),%rsi        # 0x40b348
   402415:	call   *%rsi
   402417:	mov    $0x2,%ecx
   40241c:	mov    %eax,%ebx
   40241e:	call   *0x3d0c(%rip)        # 0x406130
   402424:	mov    %ebx,%r8d
-  402427:	lea    0x4f64(%rip),%rdx        # 0x407392
+  402427:	lea    0x4f74(%rip),%rdx        # 0x4073a2
   40242e:	mov    %rax,%rcx
   402431:	call   0x404fd0
   402436:	call   *%rsi
   402438:	add    $0x40,%rsp
   40243c:	pop    %rbx
   40243d:	pop    %rsi
   40243e:	pop    %rdi
@@ -2059,15 +2059,15 @@
   40245d:	nopl   (%rax)
   402460:	mov    0x8ee1(%rip),%rsi        # 0x40b348
   402467:	call   *%rsi
   402469:	mov    $0x2,%ecx
   40246e:	mov    %eax,%ebx
   402470:	call   *0x3cba(%rip)        # 0x406130
   402476:	mov    %ebx,%r8d
-  402479:	lea    0x4f00(%rip),%rdx        # 0x407380
+  402479:	lea    0x4f10(%rip),%rdx        # 0x407390
   402480:	mov    %rax,%rcx
   402483:	call   0x404fd0
   402488:	call   *%rsi
   40248a:	add    $0x40,%rsp
   40248e:	pop    %rbx
   40248f:	pop    %rsi
   402490:	pop    %rdi
@@ -2116,15 +2116,15 @@
   402534:	jne    0x402510
   402536:	mov    0x8e0b(%rip),%rsi        # 0x40b348
   40253d:	call   *%rsi
   40253f:	mov    $0x2,%ecx
   402544:	mov    %eax,%ebx
   402546:	call   *0x3be4(%rip)        # 0x406130
   40254c:	mov    %ebx,%r8d
-  40254f:	lea    0x4e3c(%rip),%rdx        # 0x407392
+  40254f:	lea    0x4e4c(%rip),%rdx        # 0x4073a2
   402556:	mov    %rax,%rcx
   402559:	call   0x404fd0
   40255e:	call   *%rsi
   402560:	add    $0x40,%rsp
   402564:	pop    %rbx
   402565:	pop    %rsi
   402566:	pop    %rdi
@@ -2146,15 +2146,15 @@
   40258b:	nopl   0x0(%rax,%rax,1)
   402590:	mov    0x8db1(%rip),%rsi        # 0x40b348
   402597:	call   *%rsi
   402599:	mov    $0x2,%ecx
   40259e:	mov    %eax,%ebx
   4025a0:	call   *0x3b8a(%rip)        # 0x406130
   4025a6:	mov    %ebx,%r8d
-  4025a9:	lea    0x4dd0(%rip),%rdx        # 0x407380
+  4025a9:	lea    0x4de0(%rip),%rdx        # 0x407390
   4025b0:	mov    %rax,%rcx
   4025b3:	call   0x404fd0
   4025b8:	call   *%rsi
   4025ba:	add    $0x40,%rsp
   4025be:	pop    %rbx
   4025bf:	pop    %rsi
   4025c0:	pop    %rdi
@@ -2191,15 +2191,15 @@
   40262c:	jne    0x402608
   40262e:	mov    0x8d13(%rip),%rsi        # 0x40b348
   402635:	call   *%rsi
   402637:	mov    $0x2,%ecx
   40263c:	mov    %eax,%ebx
   40263e:	call   *0x3aec(%rip)        # 0x406130
   402644:	mov    %ebx,%r8d
-  402647:	lea    0x4d44(%rip),%rdx        # 0x407392
+  402647:	lea    0x4d54(%rip),%rdx        # 0x4073a2
   40264e:	mov    %rax,%rcx
   402651:	call   0x404fd0
   402656:	call   *%rsi
   402658:	add    $0x40,%rsp
   40265c:	pop    %rbx
   40265d:	pop    %rsi
   40265e:	pop    %rdi
@@ -2242,15 +2242,15 @@
   4026d5:	nopl   (%rax)
   4026d8:	mov    0x8c69(%rip),%rsi        # 0x40b348
   4026df:	call   *%rsi
   4026e1:	mov    $0x2,%ecx
   4026e6:	mov    %eax,%ebx
   4026e8:	call   *0x3a42(%rip)        # 0x406130
   4026ee:	mov    %ebx,%r8d
-  4026f1:	lea    0x4c88(%rip),%rdx        # 0x407380
+  4026f1:	lea    0x4c98(%rip),%rdx        # 0x407390
   4026f8:	mov    %rax,%rcx
   4026fb:	call   0x404fd0
   402700:	call   *%rsi
   402702:	add    $0x48,%rsp
   402706:	pop    %rbx
   402707:	pop    %rsi
   402708:	ret
@@ -2261,28 +2261,28 @@
   402716:	push   %r12
   402718:	push   %rbp
   402719:	push   %rdi
   40271a:	push   %rsi
   40271b:	push   %rbx
   40271c:	sub    $0x928,%rsp
   402723:	mov    $0xe8d,%r9d
-  402729:	lea    0x4c73(%rip),%r8        # 0x4073a3
+  402729:	lea    0x4c83(%rip),%r8        # 0x4073b3
   402730:	movl   $0x3,0x20(%rsp)
   402738:	lea    0x120(%rsp),%r14
   402740:	lea    0xa0(%rsp),%rbx
   402748:	mov    %rcx,0x970(%rsp)
   402750:	mov    %r14,%rcx
   402753:	mov    %rdx,0x978(%rsp)
   40275b:	mov    $0x400,%edx
   402760:	call   0x402360
   402765:	lea    0x50(%rsp),%r9
   40276a:	mov    %rbx,%rdx
   40276d:	mov    $0x8,%r8d
   402773:	movslq %eax,%r15
-  402776:	lea    0x4c3c(%rip),%rcx        # 0x4073b9
+  402776:	lea    0x4c4c(%rip),%rcx        # 0x4073c9
   40277d:	call   *0x8db5(%rip)        # 0x40b538
   402783:	test   %eax,%eax
   402785:	je     0x402938
   40278b:	mov    0x50(%rsp),%edx
   40278f:	cmp    $0x8,%edx
   402792:	ja     0x402920
   402798:	mov    %rbx,0x48(%rsp)
@@ -2353,39 +2353,39 @@
   4028d6:	cmp    $0xffffffffffffffff,%rax
   4028da:	je     0x402964
   4028e0:	lea    0x58(%rsp),%rax
   4028e5:	xor    %r9d,%r9d
   4028e8:	xor    %r8d,%r8d
   4028eb:	mov    %rax,0x28(%rsp)
   4028f0:	mov    0x970(%rsp),%rax
-  4028f8:	lea    0x4b19(%rip),%rdx        # 0x407418
+  4028f8:	lea    0x4b29(%rip),%rdx        # 0x407428
   4028ff:	mov    %rax,0x20(%rsp)
   402904:	call   *0x89f6(%rip)        # 0x40b300
   40290a:	add    $0x928,%rsp
   402911:	pop    %rbx
   402912:	pop    %rsi
   402913:	pop    %rdi
   402914:	pop    %rbp
   402915:	pop    %r12
   402917:	pop    %r13
   402919:	pop    %r14
   40291b:	pop    %r15
   40291d:	ret
   40291e:	xchg   %ax,%ax
-  402920:	lea    0x4ac1(%rip),%rcx        # 0x4073e8
+  402920:	lea    0x4ad1(%rip),%rcx        # 0x4073f8
   402927:	call   0x404f98
   40292c:	jmp    0x402798
   402931:	nopl   0x0(%rax)
   402938:	mov    0x8a09(%rip),%rsi        # 0x40b348
   40293f:	call   *%rsi
   402941:	mov    $0x2,%ecx
   402946:	mov    %eax,%ebx
   402948:	call   *0x37e2(%rip)        # 0x406130
   40294e:	mov    %ebx,%r8d
-  402951:	lea    0x4a68(%rip),%rdx        # 0x4073c0
+  402951:	lea    0x4a78(%rip),%rdx        # 0x4073d0
   402958:	mov    %rax,%rcx
   40295b:	call   0x404fd0
   402960:	call   *%rsi
   402962:	jmp    0x40290a
   402964:	mov    $0xffffffea,%eax
   402969:	jmp    0x40290a
   40296b:	nopl   0x0(%rax,%rax,1)
@@ -2398,15 +2398,15 @@
   402979:	push   %rbx
   40297a:	sub    $0xd0,%rsp
   402981:	lea    0x60(%rsp),%rdi
   402986:	mov    %rcx,%rsi
   402989:	mov    %rdx,%rbp
   40298c:	mov    %r8d,%r12d
   40298f:	mov    %rdx,%r9
-  402992:	lea    0x4a88(%rip),%r8        # 0x407421
+  402992:	lea    0x4a98(%rip),%r8        # 0x407431
   402999:	mov    $0x68,%edx
   40299e:	mov    %rdi,%rcx
   4029a1:	call   0x402360
   4029a6:	test   %eax,%eax
   4029a8:	js     0x402a47
   4029ae:	mov    0x895b(%rip),%r13        # 0x40b310
   4029b5:	mov    0x898c(%rip),%r14        # 0x40b348
@@ -2458,26 +2458,26 @@
   402a59:	nopl   0x0(%rax)
   402a60:	mov    0x88e1(%rip),%rsi        # 0x40b348
   402a67:	call   *%rsi
   402a69:	mov    $0x2,%ecx
   402a6e:	mov    %eax,%ebx
   402a70:	call   *0x36ba(%rip)        # 0x406130
   402a76:	mov    %ebx,%r8d
-  402a79:	lea    0x49cb(%rip),%rdx        # 0x40744b
+  402a79:	lea    0x49db(%rip),%rdx        # 0x40745b
   402a80:	mov    %rax,%rcx
   402a83:	call   0x404fd0
   402a88:	call   *%rsi
   402a8a:	jmp    0x402a47
   402a8c:	call   *%r14
   402a8f:	mov    $0x2,%ecx
   402a94:	mov    %eax,%ebx
   402a96:	call   *0x3694(%rip)        # 0x406130
   402a9c:	mov    %ebx,%r9d
   402a9f:	mov    %rbp,%r8
-  402aa2:	lea    0x497f(%rip),%rdx        # 0x407428
+  402aa2:	lea    0x498f(%rip),%rdx        # 0x407438
   402aa9:	mov    %rax,%rcx
   402aac:	call   0x404fd0
   402ab1:	mov    $0xfffffffb,%eax
   402ab6:	jmp    0x402a47
   402ab8:	nop
   402ab9:	nop
   402aba:	nop
@@ -2723,15 +2723,15 @@
   402dca:	movabs $0x1c0000409,%rax
   402dd4:	mov    %rax,0x7765(%rip)        # 0x40a540
   402ddb:	mov    0x339e(%rip),%rax        # 0x406180
   402de2:	mov    %rax,-0x10(%rbp)
   402de6:	mov    0x33a3(%rip),%rax        # 0x406190
   402ded:	mov    %rax,-0x8(%rbp)
   402df1:	call   *0x85b9(%rip)        # 0x40b3b0
-  402df7:	lea    0x4662(%rip),%rcx        # 0x407460
+  402df7:	lea    0x4672(%rip),%rcx        # 0x407470
   402dfe:	call   *0x85cc(%rip)        # 0x40b3d0
   402e04:	call   *0x8526(%rip)        # 0x40b330
   402e0a:	mov    $0xc0000409,%edx
   402e0f:	mov    %rax,%rcx
   402e12:	call   *0x85a8(%rip)        # 0x40b3c0
   402e18:	call   0x404fe8
   402e1d:	mov    0x18(%rbp),%rax
@@ -5898,130 +5898,130 @@
   407330:	js     0x40736c
   407332:	and    $0xa78342e,%eax
   407337:	add    %cl,0x70(%rdi)
   40733a:	outsb  %gs:(%rsi),(%dx)
   40733c:	imul   $0x20732520,0x67(%rsi),%ebp
   407343:	jne    0x4073b8
   407345:	imul   $0x75616220,0x67(%rsi),%ebp
-  40734c:	fs (bad)
-  40734e:	je     0x4073b5
-  407350:	cmp    $0xa7525,%eax
-  407355:	add    %al,(%rax)
-  407357:	add    %al,0x6f(%rbx)
+  40734c:	fs jb  0x4073b0
+  40734f:	je     0x4073b6
+  407351:	cmp    $0xa7525,%eax
+  407356:	add    %al,(%rax)
+  407358:	rex.XB outsl %ds:(%rsi),(%dx)
   40735a:	outsb  %ds:(%rsi),(%dx)
   40735b:	outsb  %ds:(%rsi),(%dx)
   40735c:	movsxd %gs:0x64(%rbp,%riz,2),%esi
   407361:	and    %dh,0x20(%rdi,%rbp,2)
   407365:	rex.WRB
-  407366:	gs imul $0x4d206b65,%fs:0x54(%rcx),%esp
-  40736f:	push   %rsp
-  407370:	and    $0x2078342e,%eax
-  407375:	push   %rbx
-  407376:	outsl  %ds:(%rsi),(%dx)
-  407377:	rex.XB or (%r8),%al
-  40737a:	add    %al,(%rax)
-  40737c:	add    %al,(%rax)
-  40737e:	add    %al,(%rax)
-  407380:	push   %rdi
-  407381:	jb     0x4073ec
-  407383:	je     0x4073ea
-  407385:	imul   $0x25203a29,0x28(%rbp,%r12,2),%r13d
-  40738e:	insb   (%dx),%es:(%rdi)
-  40738f:	or     %fs:(%rax),%al
-  407392:	push   %rdx
-  407393:	gs (bad)
-  407395:	imul   $0x25203a29,%fs:0x28(%rbp,%r12,2),%r13d
-  40739f:	insb   (%dx),%es:(%rdi)
-  4073a0:	or     %fs:(%rax),%al
-  4073a3:	push   %rbp
-  4073a4:	push   %rbx
-  4073a5:	rex.X pop %rsp
-  4073a7:	push   %rsi
-  4073a8:	rex.WB
-  4073a9:	rex.R pop %rdi
-  4073ab:	and    $0x2658342e,%eax
-  4073b0:	push   %rax
-  4073b1:	rex.WB
-  4073b2:	rex.R pop %rdi
-  4073b4:	and    $0x58342e,%eax
-  4073b9:	push   %rax
-  4073ba:	outsl  %ds:(%rsi),(%dx)
-  4073bb:	jb     0x407431
-  4073bd:	jae    0x4073bf
-  4073bf:	add    %dl,0x65(%rbx)
-  4073c2:	je     0x407439
-  4073c4:	jo     0x40740a
-  4073c6:	imul   $0x47737361,0x6c(%rbx),%eax
-  4073cd:	jne    0x407438
-  4073cf:	fs jae 0x407418
-  4073d2:	jb     0x407443
-  4073d4:	insl   (%dx),%es:(%rdi)
-  4073d5:	rex.WRX (bad)
-  4073d7:	insl   (%dx),%es:(%rdi)
-  4073d8:	sub    %ch,%gs:(%rcx)
-  4073db:	cmp    (%rax),%ah
-  4073dd:	and    $0xa646c,%eax
-  4073e2:	add    %al,(%rax)
-  4073e4:	add    %al,(%rax)
-  4073e6:	add    %al,(%rax)
-  4073e8:	push   %rdi
-  4073e9:	push   %r10
-  4073eb:	rex.WRX
-  4073ec:	rex.WB
-  4073ed:	rex.WRX
-  4073ee:	rex.RXB cmp (%r8),%r12b
-  4073f1:	rex.RXB push %r13
-  4073f3:	rex.WB
-  4073f4:	and    %r12b,0x6c(%rbx)
-  4073f8:	(bad)
-  4073f9:	jae    0x40746e
-  4073fb:	and    %ch,0x73(%rcx,%rbp,2)
-  4073ff:	je     0x407421
-  407401:	(bad)
-  407402:	imul   $0x74207265,0x67(%rdi),%esp
-  407409:	outsl  %ds:(%rsi),(%dx)
-  40740a:	outsl  %ds:(%rsi),(%dx)
-  40740b:	and    %ch,0x72(%rcx,%riz,2)
-  40740f:	cmp    %gs:(%eax),%ah
-  407413:	and    $0xa646c,%eax
-  407418:	push   %rax
-  407419:	outsl  %ds:(%rsi),(%dx)
-  40741a:	jb     0x407490
-  40741c:	rex.WRX (bad)
-  40741e:	insl   (%dx),%es:(%rdi)
-  40741f:	add    %bl,%gs:0x2e(%rsp,%rbx,2)
-  407424:	pop    %rsp
-  407425:	and    $0x61460073,%eax
-  40742a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-  407432:	outsl  %ds:(%rsi),(%dx)
-  407433:	jo     0x40749a
-  407435:	outsb  %ds:(%rsi),(%dx)
-  407436:	and    %al,0x4f(%rbx)
-  407439:	rex.WRB and %r14b,0x6f(%r8)
-  40743d:	jb     0x4074b3
-  40743f:	and    %ah,(%rdi)
-  407441:	and    $0x203a2773,%eax
-  407446:	and    $0xa646c,%eax
-  40744b:	rex.RXB
-  40744c:	gs je  0x407492
-  40744f:	outsl  %ds:(%rsi),(%dx)
-  407450:	insl   (%dx),%es:(%rdi)
-  407451:	insl   (%dx),%es:(%rdi)
-  407452:	push   %rbx
-  407453:	je     0x4074b6
-  407455:	je     0x4074bc
-  407457:	sub    %ch,(%rcx)
-  407459:	cmp    (%rax),%ah
-  40745b:	and    $0xa646c,%eax
-  407460:	rex movsl %ds:(%rsi),%es:(%rdi)
-  407462:	rex add %al,(%rax)
-  407465:	add    %al,(%rax)
-  407467:	add    %ah,-0x60(%rax)
-  40746a:	rex add %al,(%rax)
+  407366:	gs imul $0x53206b65,%fs:0x54(%rcx),%esp
+  40736f:	outsl  %ds:(%rsi),(%dx)
+  407370:	rex.XB cmp (%r8),%spl
+  407373:	push   $0x6f635f77
+  407378:	fs gs pop %rbx
+  40737b:	xor    %bh,0x25(%rax)
+  40737e:	cs xor $0x78,%al
+  407381:	pop    %rbp
+  407382:	or     (%rax),%al
 	...
+  407390:	push   %rdi
+  407391:	jb     0x4073fc
+  407393:	je     0x4073fa
+  407395:	imul   $0x25203a29,0x28(%rbp,%r12,2),%r13d
+  40739e:	insb   (%dx),%es:(%rdi)
+  40739f:	or     %fs:(%rax),%al
+  4073a2:	push   %rdx
+  4073a3:	gs (bad)
+  4073a5:	imul   $0x25203a29,%fs:0x28(%rbp,%r12,2),%r13d
+  4073af:	insb   (%dx),%es:(%rdi)
+  4073b0:	or     %fs:(%rax),%al
+  4073b3:	push   %rbp
+  4073b4:	push   %rbx
+  4073b5:	rex.X pop %rsp
+  4073b7:	push   %rsi
+  4073b8:	rex.WB
+  4073b9:	rex.R pop %rdi
+  4073bb:	and    $0x2658342e,%eax
+  4073c0:	push   %rax
+  4073c1:	rex.WB
+  4073c2:	rex.R pop %rdi
+  4073c4:	and    $0x58342e,%eax
+  4073c9:	push   %rax
+  4073ca:	outsl  %ds:(%rsi),(%dx)
+  4073cb:	jb     0x407441
+  4073cd:	jae    0x4073cf
+  4073cf:	add    %dl,0x65(%rbx)
+  4073d2:	je     0x407449
+  4073d4:	jo     0x40741a
+  4073d6:	imul   $0x47737361,0x6c(%rbx),%eax
+  4073dd:	jne    0x407448
+  4073df:	fs jae 0x407428
+  4073e2:	jb     0x407453
+  4073e4:	insl   (%dx),%es:(%rdi)
+  4073e5:	rex.WRX (bad)
+  4073e7:	insl   (%dx),%es:(%rdi)
+  4073e8:	sub    %ch,%gs:(%rcx)
+  4073eb:	cmp    (%rax),%ah
+  4073ed:	and    $0xa646c,%eax
+  4073f2:	add    %al,(%rax)
+  4073f4:	add    %al,(%rax)
+  4073f6:	add    %al,(%rax)
+  4073f8:	push   %rdi
+  4073f9:	push   %r10
+  4073fb:	rex.WRX
+  4073fc:	rex.WB
+  4073fd:	rex.WRX
+  4073fe:	rex.RXB cmp (%r8),%r12b
+  407401:	rex.RXB push %r13
+  407403:	rex.WB
+  407404:	and    %r12b,0x6c(%rbx)
+  407408:	(bad)
+  407409:	jae    0x40747e
+  40740b:	and    %ch,0x73(%rcx,%rbp,2)
+  40740f:	je     0x407431
+  407411:	(bad)
+  407412:	imul   $0x74207265,0x67(%rdi),%esp
+  407419:	outsl  %ds:(%rsi),(%dx)
+  40741a:	outsl  %ds:(%rsi),(%dx)
+  40741b:	and    %ch,0x72(%rcx,%riz,2)
+  40741f:	cmp    %gs:(%eax),%ah
+  407423:	and    $0xa646c,%eax
+  407428:	push   %rax
+  407429:	outsl  %ds:(%rsi),(%dx)
+  40742a:	jb     0x4074a0
+  40742c:	rex.WRX (bad)
+  40742e:	insl   (%dx),%es:(%rdi)
+  40742f:	add    %bl,%gs:0x2e(%rsp,%rbx,2)
+  407434:	pop    %rsp
+  407435:	and    $0x61460073,%eax
+  40743a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+  407442:	outsl  %ds:(%rsi),(%dx)
+  407443:	jo     0x4074aa
+  407445:	outsb  %ds:(%rsi),(%dx)
+  407446:	and    %al,0x4f(%rbx)
+  407449:	rex.WRB and %r14b,0x6f(%r8)
+  40744d:	jb     0x4074c3
+  40744f:	and    %ah,(%rdi)
+  407451:	and    $0x203a2773,%eax
+  407456:	and    $0xa646c,%eax
+  40745b:	rex.RXB
+  40745c:	gs je  0x4074a2
+  40745f:	outsl  %ds:(%rsi),(%dx)
+  407460:	insl   (%dx),%es:(%rdi)
+  407461:	insl   (%dx),%es:(%rdi)
+  407462:	push   %rbx
+  407463:	je     0x4074c6
+  407465:	je     0x4074cc
+  407467:	sub    %ch,(%rcx)
+  407469:	cmp    (%rax),%ah
+  40746b:	and    $0xa646c,%eax
+  407470:	rex movsl %ds:(%rsi),%es:(%rdi)
+  407472:	rex add %al,(%rax)
+  407475:	add    %al,(%rax)
+  407477:	add    %ah,-0x60(%rax)
+  40747a:	rex add %al,(%rax)
   40747d:	add    %al,(%rax)
   40747f:	add    %dh,0x2e(%rax)
   407482:	rex add %al,(%rax)
 	...
   4074a1:	rolb   0x0(%rax)
   4074a4:	add    %al,(%rax)
   4074a6:	add    %al,(%rax)
```

## Comparing `genio_bootrom-1.1.6.dist-info/LICENSE` & `genio_bootrom-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genio_bootrom-1.1.6.dist-info/METADATA` & `genio_bootrom-1.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genio-bootrom
-Version: 1.1.6
+Version: 1.1.7
 Summary: Tool to bootstrap the flashing on MediaTek Genio SoCs
 Home-page: https://gitlab.com/mediatek/aiot/bsp/genio-bootrom
 Author: Fabien Parent
 Maintainer: Pablo Sun
 Maintainer-email: pablo.sun@mediatek.com
 License: UNKNOWN
 Platform: UNKNOWN
```

## Comparing `genio_bootrom-1.1.6.dist-info/RECORD` & `genio_bootrom-1.1.7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 aiot_bootrom/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aiot_bootrom/bootrom.py,sha256=eYgBS7AK30n_dhXMjq7xlOH6lZc5sbUOnymiwxRoeuY,488
-aiot_bootrom/bin/bootrom-tool,sha256=y6XAykD9iNyF3xAihJM_Or6QDUwE5ChJ6YrWiIXg2xU,18712
-aiot_bootrom/bin/bootrom-tool.exe,sha256=GTkxBh7Kx_4B0AziDct7Lq80YX6IUnUf6vzTAPEg2mY,29696
-genio_bootrom-1.1.6.dist-info/LICENSE,sha256=6g4Fy_3vs1oHJZ5JlibWDFz78RmsVyAP0-jM9QLPyLw,25160
-genio_bootrom-1.1.6.dist-info/METADATA,sha256=0i01JGVEype7vlAuNrx3rexf7CgIG6SOemsrNrRmZ9I,593
-genio_bootrom-1.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genio_bootrom-1.1.6.dist-info/entry_points.txt,sha256=c8bNnOARKjd5z16RLz_LicH64BbZSxyTup-j_JJLRkI,102
-genio_bootrom-1.1.6.dist-info/top_level.txt,sha256=GfyLfW5fC5LtqHnID8unKIbDXpDXLx4liUJjk5NRYi0,13
-genio_bootrom-1.1.6.dist-info/RECORD,,
+aiot_bootrom/bin/bootrom-tool,sha256=Vvxm2vUx9C1coSfy99kdWNCE_qOdNSQTAbdKSZqonbk,18712
+aiot_bootrom/bin/bootrom-tool.exe,sha256=rnmrVz2pHJVXqjNQ8ajSTchgoLa1DMOWJ9SuhW5etv4,29696
+genio_bootrom-1.1.7.dist-info/LICENSE,sha256=6g4Fy_3vs1oHJZ5JlibWDFz78RmsVyAP0-jM9QLPyLw,25160
+genio_bootrom-1.1.7.dist-info/METADATA,sha256=DvKtMeHpv85ujGRzYDvMiXF7iPp-251GTf4thIaay08,593
+genio_bootrom-1.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genio_bootrom-1.1.7.dist-info/entry_points.txt,sha256=c8bNnOARKjd5z16RLz_LicH64BbZSxyTup-j_JJLRkI,102
+genio_bootrom-1.1.7.dist-info/top_level.txt,sha256=GfyLfW5fC5LtqHnID8unKIbDXpDXLx4liUJjk5NRYi0,13
+genio_bootrom-1.1.7.dist-info/RECORD,,
```

