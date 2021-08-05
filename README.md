# 行列 10 鍵數字輸入法表格
(Tables of Array10 Numeric Input Method)

這是提供給 LIME for Android 的「行列10」輸入法表格，其中 array10a 已內建在 LIME 中，使用者無需再重覆匯入。

**釋出說明：**

本輸入法表格係由行列科技公司廖明德先生（即行列輸入法發明人）提供原始對照表，經葉光哲先生（老刀）與廖先生共同修正編訂。

「行列 10 數字輸入法」（以下簡稱「行列 10」）係為行列 30 鍵輸入法（以下簡稱「行列 30」）字根數字化的衍生版本，二者對於文字拆碼方式基本上是相同的。主要差異為使用 1234567890 共 10 個數字鍵輸入字根碼，來代替行列 30 中的鍵盤鍵位。本 1.0A 版本支援 Unicode 3.0 範圍（亦即包括中日韓統一表意文字延伸 A 區 (Ext-A)），共二萬七千餘漢字。

註：本輸入法另提供支援 Unicode 3.1 範圍漢字（亦即包括中日韓統一表意文字延伸 B 區 (Ext-B)）的版本，版本號碼為 v1.0B。

「行列 10」與「行列 30」相異之處，說明如下：

1. 輸入文字時，行列 30 係以「鍵位」代表字根，如字根「日」之字根碼為 01，即對應到英文鍵盤的 "P" 鍵；而行列 10 為直接輸入字根碼 (01)（其餘字根均依此類推）。
1. 單字根碼僅按單鍵（行列 30 的字根碼 1-，在行列 10 中僅按單鍵 (1) 即可），前後皆不補鍵。
1. 輸入罕用字時，行列 10 無需於字根尾補 "I" 鍵。
1. 行列 30 每個漢字最多拆 4 個字根（不含罕用字補 "I"）。因行列 10 採直接輸入字根碼的方式，故對每個漢字而言，無論是否為罕用字，最多拆 8 個數字。
1. 行列 10 亦保留輸入原先行列 30 的標點及符號組的功能。請以字根碼 (23)（即相當於鍵盤的 "W" 鍵）作為前導，第 3 碼為符號分組，如 (231) 輸入標點、(232) 輸入括弧、(233) 輸入一般符號……(230) 輸入注音符號，分組方式與行列 30 相同。
1. 為方便使用者更快速輸入標點及符號，於上述 (231) ~ (230) 10組之下再設支碼。如輸入 (231) 標點符號組時，(2311) 是該組第 1 頁的 10 個符號，(2312) 則是該組的第 2 頁的 10 個符號……（餘類推）。故當使用者熟知要的符號是標點符號的第幾頁後，就可以直接打 4 碼快速找到，例如要輸入「■」符號時，只要打 (2312) 再選第 7 個，如果不熟，打 (231) 3 碼再往後找，同樣可以找到。
1. 行列 10 新增輸入全形英文字母及數字的功能，並編入字根碼 (255)。當輸入 (255) 時即可自候選字窗選取，或亦可再輸入第 4 碼（分組支碼），以縮短選取全形文字所需時間。說明如下：
    * (2551)：全形英文字母Ａ至Ｊ，共 10 個。
    * (2552)：全形英文字母Ｋ至Ｔ，共 10 個。
    * (2553)：全形英文字母Ｕ至Ｚ，共 6 個。
    * (2554)：全形英文字母ａ至ｊ，共 10 個。
    * (2555)：全形英文字母ｋ至ｔ，共 10 個。
    * (2556)：全形英文字母ｕ至ｚ，共 6 個。
    * (2550)：全形數字０至９，共 10 個。

本輸入法為將行列字根數字化，部分文字的拆法（尤其是輸入標點符號方面）與原行列 30 鍵輸入法相較，已略有調整。故在此將廖明德先生發行原始對照表的註解摘錄整理於下，提供各位參考：

> 1. 本檔案已依照字頻序排列（前加幾個常用符號）。
> 1. 字頻資訊是以平衡語料庫加網路論壇的字頻統計資料綜合而成，以兼顧一般運用及網路上使用的均衡性。
> 1. 建議使用者使用行列數字輸入時，保持原來的想法輸入，如「二」字，雖然是輸入 (11)，但心裡還是想著 (1- 1-) 即默念（1單1單），只有在輸入「工」字時，才是想 (11)，這樣回到 30 鍵盤上才不會亂掉。
> 1. 本行列數字輸入法最多為 4 根 8 數碼（未加罕用區別碼）。因對照表以字頻排序，故程式接到敲鍵後宜以依序抓取，順序顯示待選字的方式處理，若再接收到下一個鍵，則再篩掉不合的字，保留符合的字，如此應該大部份的字都在敲 4 或 5 個數字鍵內就會出現供使用者選取。要注意這種情形，如「龜」有 (7711)、(77151)、(77198)、(7712) 四種拆法，使用者一直敲到第三個鍵 (771) 時，在對照表內符合的抓出來會有四個「龜」字，但只需顯示一個「龜」字，（當然 4 組編碼都要保留等待下一鍵進來比對）。
> 1. 非常用字的單根碼轉變成 4 根碼（4 根最多 8 碼）置於後段。
> 1. 編 (09) 開頭的特殊符號 09？  09『  09』 09． 09– 09＊ 09／ 09…
> 1. 編為 (09) 開頭是為了避開和 (08) 開頭的常用字混在一起。且 09 和 08 回到 30鍵時是同一鍵位。
> 1. 編 (35) 開頭的 35片 35 岩 35！ 35「 35」 35、 35“  35 ”35（ 35）
> 1. 編十組符號以 (23)（代替W）前導，(231)（標點）、(232)（括號）、(233)（一般）、(234)（數學）……等，共十組。
> 1. 數字編碼以 (23) 為十組符號的前導碼，因 (23) 沒有字根，位置一樣在 W，用它為前導碼就不會跟字混雜顯現，且使用者回到 30 鍵上輸入能夠保持一致。
> 1. 行列數字輸入應以隨著資訊增加漸縮符合字集的方式顯示待選字，在特殊符號的部份因每組符號有幾十個，因此配合漸縮字集方式設計成：
>
>    * 當輸入 (231) 標點符號組，(2311) 是該組第 1 頁的十個符號，(2312) 則是該組的第 2 頁的十個符號……餘類推。
>    * 當使用者熟知要的符號是標點符號的第幾頁後，就可以直接打 4 碼快速找到，例如要「■」符號，只要打 (2312) 再選第 7 個，如果不熟，打 (231) 3 碼再往後找也是找得到。

**版權聲明：**

本輸入法表格版權，屬廖明德先生與葉光哲先生共有。惟依行列輸入法公開授權使用之精神，歡迎各位朋友引用、散布（複製）。為使本輸入法符合各家作業平台及使用環境，亦歡迎使用者修改本檔案；惟請於所修改之原始檔或說明文字中，註明檔案來源及版次資訊（如：「本輸入法係修改自行列 10 數字輸入法 (array10 numeric) for LIME, v1.0A」），以因應未來本輸入法表格版本後續更新時，可提醒修正者或使用者配合維護。
