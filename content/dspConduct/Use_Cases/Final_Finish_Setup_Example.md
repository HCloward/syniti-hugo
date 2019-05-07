+++
title = 'Final Finish Setup Example'
solution = 'Master Data Management'
+++

# Final Finish Setup Example

A Designer sets up the final finish for the single table KNA1 registered
to Task Request (Address – General), with a source of RD2 and a target
of dgSAP.<span> </span>

<span>![](../../../Resources/Images/clip_image001.png)</span>

In database DGE\_Data, table ttKNA1\_ADRC KUNNR value for a specific
RequestID will provide the data for KUNNR value that will be used to
form the SELECT statement.

<span>![](../../../Resources/Images/clip_image003.jpg)</span>

After posting, the KUNNR value in table ttKNA1\_ADRC is 0000001718*.*

The resulting SELECT statement that is executed is:

 

<span style="background: #DEE2E7;">Select \[MANDT\], \[KUNNR\],
\[LAND1\], \[NAME1\], \[NAME2\], \[ORT01\], \[PSTLZ\], \[REGIO\],
\[SORTL\], \[STRAS\], \[TELF1\], \[TELFX\], \[XCPDK\], \[ADRNR\],
\[MCOD1\], \[MCOD2\], \[MCOD3\], \[ANRED\], \[AUFSD\], \[BAHNE\],
\[BAHNS\], \[BBBNR\], \[BBSNR\], \[BEGRU\], \[BRSCH\], \[BUBKZ\],
\[DATLT\], \[ERDAT\], \[ERNAM\], \[EXABL\], \[FAKSD\], \[FISKN\],
\[KNAZK\], \[KNRZA\], \[KONZS\], \[KTOKD\], \[KUKLA\], \[LIFNR\],
\[LIFSD\], \[LOCCO\], \[LOEVM\], \[NAME3\], \[NAME4\], \[NIELS\],
\[ORT02\], \[PFACH\], \[PSTL2\], \[COUNC\], \[CITYC\], \[RPMKR\],
\[SPERR\], \[SPRAS\], \[STCD1\], \[STCD2\], \[STKZA\], \[STKZU\],
\[TELBX\], \[TELF2\], \[TELTX\], \[TELX1\], \[LZONE\], \[XZEMP\],
\[VBUND\], \[STCEG\], \[DEAR1\], \[DEAR2\], \[DEAR3\], \[DEAR4\],
\[DEAR5\], \[GFORM\], \[BRAN1\], \[BRAN2\], \[BRAN3\], \[BRAN4\],
\[BRAN5\], \[EKONT\], \[UMSAT\], \[UMJAH\], \[UWAER\], \[JMZAH\],
\[JMJAH\], \[KATR1\], \[KATR2\], \[KATR3\], \[KATR4\], \[KATR5\],
\[KATR6\], \[KATR7\], \[KATR8\], \[KATR9\], \[KATR10\], \[STKZN\],
\[UMSA1\], \[TXJCD\], \[PERIV\], \[ABRVW\], \[INSPBYDEBI\],
\[INSPATDEBI\], \[KTOCD\], \[PFORT\], \[WERKS\], \[DTAMS\], \[DTAWS\],
\[DUEFL\], \[HZUOR\], \[SPERZ\], \[ETIKG\], \[CIVVE\], \[MILVE\],
\[KDKG1\], \[KDKG2\], \[KDKG3\], \[KDKG4\], \[KDKG5\], \[XKNZA\],
\[FITYP\], \[STCDT\], \[STCD3\], \[STCD4\], \[XICMS\], \[XXIPI\],
\[XSUBT\], \[CFOPC\], \[TXLW1\], \[TXLW2\], \[CCC01\], \[CCC02\],
\[CCC03\], \[CCC04\], \[CASSD\], \[KNURL\], \[J\_1KFREPRE\],
\[J\_1KFTBUS\], \[J\_1KFTIND\], \[CONFS\], \[UPDAT\], \[UPTIM\],
\[NODEL\], \[DEAR6\], \[/VSO/R\_PALHGT\], \[/VSO/R\_PAL\_UL\],
\[/VSO/R\_PK\_MAT\], \[/VSO/R\_MATPAL\], \[/VSO/R\_I\_NO\_LYR\],
\[/VSO/R\_ONE\_MAT\], \[/VSO/R\_ONE\_SORT\], \[/VSO/R\_ULD\_SIDE\],
\[/VSO/R\_LOAD\_PREF\], \[/VSO/R\_DPOINT\], \[ALC\], \[PMT\_OFFICE\],
\[PSOFG\], \[PSOIS\], \[PSON1\], \[PSON2\], \[PSON3\], \[PSOVN\],
\[PSOTL\], \[PSOHS\], \[PSOST\], \[PSOO1\], \[PSOO2\], \[PSOO3\],
\[PSOO4\], \[PSOO5\] From \[rd2\].\[KNA1\]  Where \[MANDT\] = '120'  AND
KUNNR IN ('0000001718' )</span>

 

A Designer can also set up download for a table with multiple keys. As
an example of a setup for table ADCP registered to Task Request (Contact
Person) source = RD2, target = dgSAP.<span> </span> ADCP requires two
key values, ADDRNUMBER and PERSNUMBER.

 

<span>![](../../../Resources/Images/clip_image005.jpg)</span>

 

In database DGE\_Data, for a specific RequestID, view
webRequestRole\_Finish\_ContactAddressSel will provide the ADRNR data
for ADDRNUMBER value and the PRSNR data for PERSNUMBER value that will
be used to form the SELECT statement.

 

 <span>![](../../../Resources/Images/clip_image007.jpg)</span>

After Posting, the resulting values from the view
webRequestRole\_Finish\_ContactAddressSel are ADRNR = 0000026044 and
PRSNR = 0000026044.

The resulting SELECT statement that is executed is:

 

<span style="color: #525152;background: #DEE2E7;">Select \[CLIENT\],
\[ADDRNUMBER\], \[PERSNUMBER\], \[DATE\_FROM\], \[NATION\],
\[DATE\_TO\], \[COMP\_PERS\], \[SO\_KEY\], \[DEPARTMENT\], \[FUNCTION\],
\[BUILDING\], \[FLOOR\], \[ROOMNUMBER\], \[ID\_CODE\], \[IH\_MAIL\],
\[SORT1\], \[SORT2\], \[SORT\_PHN\], \[ALT\_COMPNY\], \[DEFLT\_COMM\],
\[TEL\_NUMBER\], \[TEL\_EXTENS\], \[FAX\_NUMBER\], \[FAX\_EXTENS\],
\[FLAGCOMM2\], \[FLAGCOMM3\], \[FLAGCOMM4\], \[FLAGCOMM5\],
\[FLAGCOMM6\], \[FLAGCOMM7\], \[FLAGCOMM8\], \[FLAGCOMM9\],
\[FLAGCOMM10\], \[FLAGCOMM11\], \[FLAGCOMM12\], \[FLAGCOMM13\] From
\[rd2\].\[ADCP\]  Where \[CLIENT\] = '120'  AND PERSNUMBER IN
('0000026045' ) AND ADDRNUMBER IN ('0000026044' )</span>
