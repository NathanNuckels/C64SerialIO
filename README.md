# C64SerialIO
Raw Serial port IO for commodore 64



- [ ] Figure how how to acess function peramiters in assembly
  - [ ] Assembly to Assembly `jsr XX`
  - [ ] C to Assembly `function(XX);`
  - [ ] Assembly to C `return XX;`
- [ ] Start by making a library to expose kernel subroutines
  - [ ] `void cbm_TALK(char device)`
  - [ ] `void cbm_LISTEN(char device)`
  - [ ] `void cbm_UNTLK()`
  - [ ] `void cbm_UNLSN()`
  - [ ] `void cbm_SETLFS(char fd,char device,char seccond)` (ASM)
  - [ ] `void cbm_SETNAM(char * name, char name_length)` (ASM)
  - [ ] `char cbm_OPEN()` (ASM)
  - [ ] `char cbm_CLOSE(char fd)`
  - [ ] `char cbm_CHKIN(char fd)`
  - [ ] `char cbm_CHKOUT(char fd)`
  - [ ] `void cbm_CHROUT(char cout)`
  - [ ] `char cbm_CHRIN()`
  - [ ] `char cbm_GETIN()`
- [ ] Make higher level things for disk drive files
  - [ ] `char dos_fdopen(char fd,char * name,char mode,char type,char disk)` (C)
  - [ ] `char dos_fopen(char * name,char mode,char type,char disk)` (C)
  - [ ] `char dos_fdclose()` (C)
  - [ ] `char read_char(char fd)` (C)
  - [ ] `char * read_line(char fd)` (C)
  - [ ] `char * read_all(char fd)` (C)
  - [ ] `char write_char(char fd,char data)` (C)
  - [ ] `char write_string(char fd,char * data,char length)` (C)

# Other general usefull stuff
- [ ] Dynamic memory allocation `<stdlib.h>`
- [ ] String utils `<string.h>`

# `libc_cc65` stuff
- [ ] `__EXEHDR__`
- [ ] `__LOADADDR__`
