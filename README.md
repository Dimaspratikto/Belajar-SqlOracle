# Belajar-SqlOracle
# 1.BUAT TABLESPACE
CREATE TABLESPACE COMPANY DATAFILE 'C:\FILEKU\Belajar\TBSPACE-SQL\TBCOMPANY.DBF' SIZE 10M;

# 2.PASTIKAN SUDAH CONN SYSTEM UNTUK MEMBUAT USER
alter session set "_ORACLE_SCRIPT"=true;

# 3.BUAT USER
create user ptberkah
identified by 1234
default tablespace company
quota unlimited on company;