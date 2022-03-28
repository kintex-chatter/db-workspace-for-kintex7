# workspace for prjxray DB for kintex7

A workspace for @hansfbaier's prjxray DB / kintex7.

## ChangeLog

* Add xc7k325tffg676-1 from the old database.

* Remove a (suspicious) conflicting bit

```
prjxray.fasm_assembler.FasmInconsistentBits: FASM line "INT_R_X95Y132.IMUX34.SL1END1" wanted to set bit (4206489, 65, 21) but was cleared by FASM line "RIOB18_X95Y131.IOB_Y0.SSTL135.DRIVE.I_FIXED"
```
-> Drop !25_85 from RIOB18.IOB_Y0.SSTL135.DRIVE.I_FIXED.

* Add the missing lines to segbits_rioi.db/segbits_rioi_tbyteterm.db from @hansfbaier's 20220326 DB.

* Add a fake ppips_rioi_tbyteterm.db which is created from ppips_rioi3_tbyteterm.db.

* Fill the empty "bits" of LIOI3_X0Y9 with the content of "bits" of LIOB33_X0Y9.
