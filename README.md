# 行列 10 鍵數字輸入法表格
(Array10 Numeric Input Method Tables)

這是提供給 LIME for Android 的「行列10」輸入法表格。

* /LIME：專為 LIME for Android 設計的「行列10」輸入法表格檔。
* /OpenVanilla：專為 OpenVanilla for macOS 設計的「行列10」輸入法表格檔。
* /gcin：專為 gcin 設計的「行列10」輸入法鍵碼表。

## 行列10 輸入法簡介、使用指引及版權聲明
請參考本站的 [wiki 頁面](https://github.com/gontera/array10/wiki/%E8%A1%8C%E5%88%9710%E9%8D%B5%E6%95%B8%E5%AD%97%E8%BC%B8%E5%85%A5%E6%B3%95%E8%AA%AA%E6%98%8E%E5%8F%8A%E6%8C%87%E5%BC%95%E9%A6%96%E9%A0%81)。

## 鍵碼表匯入教學
### LIME
[請點此參考](https://github.com/gontera/array30/wiki/LIME-%E6%95%99%E5%AD%B8-(1)%EF%BC%9A%E5%A6%82%E4%BD%95%E5%9C%A8-LIME-%E4%B8%8A%E9%9D%A2%E5%8C%AF%E5%85%A5%E6%96%B0%E7%89%88%E7%9A%84%E8%A1%8C%E5%88%97%E9%8D%B5%E7%A2%BC%E8%A1%A8)。
### gcin 
[請點此參考](https://github.com/gontera/array30/wiki/gcin-for-Android-%E6%95%99%E5%AD%B8-(3)%EF%BC%9A%E6%8E%9B%E8%BC%89%E6%96%B0%E7%89%88%E8%A1%8C%E5%88%97%E8%BC%B8%E5%85%A5%E6%B3%95%E6%A8%A1%E7%B5%84)。

## 版本釋出說明
版本：v2023-1.0，釋出日期：2023-02-11

行列10鍵數字輸入法（下稱「行列10」）對照表自從 2010 年首次釋出 (array10a/b) 之後，近 13 年來僅對於少部分錯植的字根編碼予以更正，基本上沒有重大更新。本次更新係為配合行列輸入法30鍵版（行列30）v2023 版校編工作，對於行列10鍵碼表亦同步展開校編的成果。

### 參照多字體重新校編
中日韓統一表意文字包括中（繁/簡）日、韓、越的漢字集，本次更新已全面支援中日韓統一表意文字延伸 G 區 (Ext-G)，符合 Unicode 14.0 規格，並已籌備對於延伸 H 區的編碼支援。此外，亦在儘量不影響原使用習慣的原則下，參考多種現普遍流通的漢字字型重新校編既有漢字，以兼顧各漢字族群的使用者。

對於同 Unicode 內碼卻顯示字型分歧的處理上，係以不增加大量重複字為前提，儘量支援各種字型的定義；但若會造成大量重複字的，則以列表讓使用者有所依循，不會依字型打不出字來。
本次校編所參考的字型，計有：微軟標楷體、微軟新細明體、微軟新細明體 Ext-B、微軟黑體、思源黑體、思源宋體台灣、花園明朝體（HanaMinA/HanaMinB），也包括早期參考的華康和文鼎字體等。

### 行列10鍵碼表的版本
本次行列10鍵碼表依據蒐錄的字集範圍區分，計釋出 3 組版本。除先前已有的 array10a 及 array10b 兩組之外，再增加 array10c 一組，說明如下：
1. array10a：支援包括中日韓統一表意文字延伸 A 區 (Ext-A) 共二萬七千餘漢字的「標準版」。如將鍵碼表匯入手機使用，建議以此版本匯入，將帶來最佳的使用者體驗，亦最節省使用手機有限的記憶空間。
1. array10b：除蒐錄 array10a 的內容外，尚包括中日韓統一表意文字延伸 B 區 (Ext-B)，合計七萬餘字。因現階段尚無任何廠牌型號智慧手機及 iPad 或 Android 平板電腦之內建字型可以完整支援 Ext-B 範圍的定義（亦即在 Ext-B 區段會有大量以「〿」符號代表的缺字），除非您真的有在手機輸入這些文字的需求，否則不建議匯入使用。當然，如您將手機打好的文字轉貼到安裝有適當字型的個人電腦系統（如 Windows、macOS及各種 Linux distros 等）上，應該就可以顯示原本應顯示的文字。
1. array10c：為包括中日韓統一表意文字延伸 G 區 (Ext-G)，合計九萬二千餘字（c 代表 "Complete Set"，即蒐錄的範圍為「全字集」之意），蒐錄的字集範圍最廣、字數最多。不建議在手機上使用，係提供輸入法開發者將行列10移植到個人電腦系統，或做為研究行列10輸入法之用。

### 支援字集的更動
本次校編已將中日韓統一表意文字及其各延伸字面的缺字予以補足。其中在中日韓統一表意文字範圍增補 90 字（內碼 U+9FA6-U+9FFF）及延伸 A 區 (Ext-A) 增補 10 字（內碼 U+4DB6-U+4DBF）(array10a/b)、延伸 B 區 (Ext-B) 增補 9 字（內碼 U+2A6D7-U+2A6DF）(array10b)。

本次校編亦遵循 Unicode 1.1 的定義，在(0) 及特別碼 (071) 皆以漢字零（〇，內碼 U+3007）取代原有符號圈（○，內碼 U+25CB）。如要輸入符號圈，請回歸 (2331) 的第 7 個。

### (23) 符號選單
行列10的 (23) 符號選單，提供方便快速輸入符號的捷徑，是頗受使用者歡迎的功能。配合行列30輸入法 v2023 的更新，亦同步採用全新的符號選單，增添下列功能：
1. (233) 一般符號：增加右三角形（U+25B7，▷；U+25BA，►）及左三角形（U+25C1，◁；U+25C4，◄）。
1. (236) 單位符號：新增貨幣符號（U+20AC，歐元 €；U+FFE6，韓元 ￦），並大幅擴充物理單位符號。
1. (237) 圖表符號：新增 U+2591，░ 及 U+2592，▒。
1. (238) 順序符號：現在已有更多組標號字符可供選擇，並擴充若干組標號字符至 20 號。
