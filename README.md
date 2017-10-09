# The Adobe-CNS1-7 Character Collection
---
© 1995, 1998, 2000, 2001, 2003, 2005, 2007, 2009, 2012, 2017 Adobe Systems Incorporated.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file to use, copy, publish, distribute, sublicense, and/or sell copies of the documentation, and to permit others to do the same, provided that:

No modification, editing or other alteration of this document is allowed; and

The above copyright notice and this permission notice shall be included in all copies of the documentation.

Permission is hereby granted, free of charge, to any person obtaining a copy of this documentation file, to create their own derivative works from the content of this document to use, copy, publish, distribute, sublicense, and/or sell the derivative works, and to permit others to do the same, provided that the derived work is not represented as being a copy or version of this document.

Adobe shall not be liable to any party for any loss of revenue or profit or for indirect, incidental, special, consequential, or other similar damages, whether based on tort (including without limitation negligence or strict liability), contract or other legal or equitable grounds even if Adobe has been advised or had reason to know of the possibility of such damages. The Adobe materials are provided on an "AS IS" basis. Adobe specifically disclaims all express, statutory, or implied warranties relating to the Adobe materials, including but not limited to those concerning merchantability or fitness for a particular purpose or non-infringement of any third party rights regarding the Adobe materials.

Adobe holds no patents on the subject matter of this specification.

Last updated 2017-10-09

---
## Introduction
The purpose of this document is to define and describe the *Adobe-CNS1-7* character collection, which enumerates 19,179 glyphs, and whose designation is derived from the following three /CIDSystemInfo dictionary entries:

* /Registry (Adobe)
* /Ordering (CNS1)
* /Supplement 7

CIDFont resources that reference this character collection must include a /CIDSystemInfo dictionary that matches the /Registry and /Ordering strings shown above.

This document is designed for font developers, for the purpose of developing Traditional Chinese fonts for use with PostScript products, or for developing OpenType Traditional Chinese fonts. It is also useful for application developers and end users who need to know more about the glyphs in this character collection. This document expects that its readers are familiar with the CID-keyed font file format, which is described in [Adobe Technical Note #5014](https://www.adobe.com/devnet/font.html), entitled *Adobe CMap and CIDFont Files Specification*.

A character collection contains the glyphs that are required to develop font products for a specific language, script, or market. Specific encodings are defined through the use of CMap resources that are instantiated as files, and generally reference a subset of the character collection.

The character collection that results from each Supplement includes the glyphs associated with all earlier Supplements. For example, Supplement 7 includes all glyphs defined in Supplements 0 through 6.

The Adobe-CNS1-7 character collection enumerates 19,179 glyphs, specifically CIDs 0 through 19178, among eight Supplements, designated 0 through 7. Adobe-CNS1-6 supports CNS 11643 Planes 1 and 2, Big Five, Hong Kong GCCS, and the 1999, 2001, 2004, 2008, and 2016 versions of [Hong Kong SCS](https://www.ogcio.gov.hk/en/business/tech_promotion/ccli/hkscs/) (*Hong Kong Supplementary Character Set* or shortened to HKSCS). The following table summarizes these eight Supplements, and also provides the pages on which their glyphs are shown in the [*Adobe-CNS1-7.pdf*](https://github.com/adobe-type-tools/Adobe-CNS1/raw/master/Adobe-CNS1-7.pdf) file:

**Supplement** | **Additional CIDs** | **CID Range** | **Total CIDs** | **Date of Establishment** | **Pages**
--- | --- | --- | --- | --- | ---
0 | *n/a* | 0–14098 | 14,099 | 1995-06-26 | 1–29
1 | 3,309 | 14099–17407 | 17,408 | 1998-09 | 29–35
2 | 193 | 17408–17600 | 17,601 | 1998-10-12 | 35–36
3 | 1,245 | 17601–18845 | 18,846 | 2000-06 | 36–38
4 | 119 | 18846–18964 | 18,965 | 2001-08 | 38
5 | 123 | 18965–19087 | 19,088 | 2005-07-08 | 38–39
6 | 68 | 19088–19155 | 19,156 | 2009-09-24 | 39
7 | 23 | 19156–19178 | 19,179 | 2017-07-04 | 39

Each CID (*Character ID*) in a character collection is associated with a class of character shapes or glyphs. The specific shape of a glyph from a given glyph class is dependent on the typeface style and possibly other factors. Glyphs for all CIDs are illustrated in this document, providing a specific example or instance of the correspondence between a CID and its glyph shape class. Font developers should design glyphs for each CID of the character collection, and may use this document as a reference when proofing or otherwise validating CIDFont resources.

The following sections detail the history and contents of each of the eight Supplements of the Adobe-CNS1-7 character collection.

---
## Supplement 0—Adobe-CNS1-0

Supplement 0, which enumerates 14,099 glyphs, specifically CIDs 0 through 14098, supports the CNS 11643-1992 character set standard (Planes 1 and 2 only), Big Five, and the ETen extensions to Big Five.

---
## Supplement 1—Adobe-CNS1-1

Supplement 1 provides 3,309 additional glyphs, specifically CIDs 14099 through 17407, that are necessary to support Hong Kong GCCS and its extension, along with vendor-specific character sets from Monotype and DynaComware. CIDs 14099 through 14122 are punctuation and line-drawing glyphs, which have been included to completely support the needs of vertical and horizontal writing modes.

---
## Supplement 2—Adobe-CNS1-2

Supplement 2 adds 193 glyphs, specifically CIDs 17408 through 17600, and was designed to add only pre-rotated versions of all non–full-width Latin and Latin-like glyphs found in Supplement 1 and earlier, for the specific purpose of supporting the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB (*Glyph SUBstitution*) feature.

---
## Supplement 3—Adobe-CNS1-3

Supplement 3 adds 1,245 glyphs, specifically CIDs 17601 through 18845. Glyphs for the Euro currency symbol are at CIDs 17601 through 17605 (proportional, full-width, and half-width Euro glyphs, along with pre-rotated proportional and half-width Euro glyphs). Also included are those glyphs necessary to fully support Hong Kong SCS as initially published by the goverment of the Hong Kong Special Administrative Region (SAR) of the People’s Republic of China (Hong Kong SCS-1999). Glyphs for hanzi that were not already included in Adobe-CNS1-1 are allocated at CIDs 17606 through CIDs 18784. CIDs 18785 through 18845 complete the support for Hong Kong SCS by allocating positions for Latin or Latin-like glyphs with diacritic marks, along with additional symbols.

---
## Supplement 4—Adobe-CNS1-4

Supplement 4 adds 119 glyphs, specifically CIDs 18846 through 18964. 116 of these glyphs (CIDs 18849 through 18964) have been added to reflect the addition of 116 characters, all of which are hanzi, to Hong Kong SCS-2001.
CIDs 18846, 18847, and 18848 are necessary to distinguish the designs of three Hong Kong SCS characters (0xC8E0, 0xC8E9, and 0xC8F1) versus the designs of three Big Five characters (0xA4EB, 0xA8A4, and 0xF0E8). In the past, the former three characters were rendered using CIDs 732, 1289, and 2550, because they were considered to be identical with the latter. However, the purpose of the three Hong Kong SCS characters is to represent three Unicode “CJK Radicals Supplement” characters (U+2E9D &#x2E9D;, U+2EC6 &#x2EC6;, and U+2EE3 &#x2EE3;). This led to design adjustments that necessitated the addition of CIDs 18846, 18847, and 18848.

---
## Supplement 5—Adobe-CNS1-5

Supplement 5 adds 123 new glyphs, specifically CIDs 18965 through 19087, to reflect the addition of 123 characters, all of which are hanzi, to Hong Kong SCS-2004.

---
## Supplement 6—Adobe-CNS1-6

Supplement 6 adds 68 new glyphs, specifically CIDs 19088 through 19155, to reflect the addition of 68 characters, all of which are hanzi, to Hong Kong SCS-2008.

---
## Supplement 7—Adobe-CNS1-7

Supplement 7 adds 23 new glyphs, specifically CIDs 19156 through 19178, to reflect the addition of 23 characters, all of which are hanzi, to Hong Kong SCS-2016. Hong Kong SCS-2016 also added the Euro currency symbol, whose glyphs were already included in Supplement 3.

---
## Special Glyphs & Other Notes
The following sections detail special glyphs and other notes that are of interest to font developers. Several glyph classes are complex, and deserve some amount of explanation and clarification.

### Space Glyphs

The following table lists all of the Adobe-CNS1-7 glyphs that are classified as a space, or are otherwise rendered as a space, and provides information with regard to their intended usage, along with their recommended set widths:

**CID** | **Set Width** | **Description**
--- | --- | ---
1 | Proportional | Latin space—U+002099 | Full-width | Ideographic space—U+300013648 | Half-width | Latin space—U+200217408 | Full-width | Pre-rotated version of CID+117506 | Full-width | Pre-rotated version of CID+13648

The space glyphs that are described as a pre-rotated version of another glyph must be assigned full-width set widths in terms of their horizontal set widths, but when instantiated as an OpenType font, their vertical set widths as specified in the OpenType ‘[vmtx](https://www.microsoft.com/typography/otspec/vmtx.htm)’ (*Vertical Metrics*) table should match those of their unrotated counterparts.

### Hanzi Glyphs

Adobe-CNS1-7 includes 17,898 glyphs that are classified as hanzi (aka ideographs), and their CID ranges, separated by Supplement, are shown in the table below:

**Supplement** | **CID Ranges**
--- | ---
0 | 281–289, 536–561, 595–13645, 13999–14008, 14056–140621 | 14123–174072 | *none*3 | 17608–187844 | 18846–189645 | 18965–190876 | 19088–19155
7 | 19156–19178

### Pre-Rotated Glyphs

In order to support the OpenType ‘[vrt2](https://www.microsoft.com/typography/otspec/features_uz.htm#vrt2)’ (*Vertical Alternates and Rotation*) GSUB feature, the Adobe-CNS1-7 character collection includes pre-rotated forms for all Latin and Latin-like glyphs that are not full-width. The table below details how horizontal CIDs and CID ranges map to their corresponding pre-rotated CID ranges:

**Supplement** | **Horizontal CIDs & CID Ranges** | **Pre-Rotated CID Ranges**
--- | --- | ---
2 | 1–98, 13648–13742 | 17408–176003 | 17601, 17603 | 17604–17605

### Glyph Set Widths

The following table provides CIDs and CID ranges that explicitly indicate which glyphs are intended to be designed with proportional- or half-width set widths. All other glyphs are expected to be full-width.

**Set Width** | **CIDs & CID Ranges**
--- | ---
Proportional | 1–98, 17601Half-width | 13648–13742, 17603
The glyph tables that are provided in this document include registration marks that serve to indicate relative set width. Explicitly specifying width classes, such as in the above table, is clearly more accurate and reliable than measuring the distance between registration marks. Please use both resources as your guide.

Note that the registration marks used in the glyph tables are in a separate layer, and if their presence is annoying, that layer can be turned off, thus preventing their display.

---
## CMap Resources

The CMap resources associated with the Adobe-CNS1-7 character collection, along with the [*cid2code.txt*](https://raw.githubusercontent.com/adobe-type-tools/cmap-resources/master/Adobe-CNS1-7/cid2code.txt) datafile that provides additional details for font developers, are available as part of the [*CMap Resources*](https://github.com/adobe-type-tools/cmap-resources/) open source project.

More complete descriptions of the individual Adobe-CNS1-7 CMap resources can be found in [Adobe Technical Note #5094](https://www.adobe.com/devnet/font.html), entitled *Adobe CJKV Character Collections and CMap Files for CID-Keyed Fonts*.

In general, the CMap resources that are based on legacy encodings, such as Big Five, are no longer being updated. Rather, the Unicode CMap resources—available for UTF-8, UTF-16 (UTF-16BE), and UTF-32 (UTF-32BE) encodings, and kept perfectly synchronized—are updated on a regular basis, with new mappings being triggered by a new Supplement or a new version of Unicode. Furthermore, the UCS-2 CMap resources are obsolete and deprecated. Developers should use the UTF-16 CMap resources instead, because they are forward compatible with the now-obsolete UCS-2 ones.

---
## Unicode Variation Sequences

The [Standardized Variation Sequences](http://www.unicode.org/Public/UCD/latest/ucd/StandardizedVariants.txt) (SVSes) that are specified in the [*Adobe-CNS1_sequences.txt*](https://github.com/adobe-type-tools/Adobe-CNS1/raw/master/Adobe-CNS1_sequences.txt) datafile correspond to CJK Compatibility Ideographs.

---
## Glyph Tables

Representative glyphs for CIDs 0 through 19178 are provided in the [*Adobe-CNS1-7.pdf*](https://github.com/adobe-type-tools/Adobe-CNS1/raw/master/Adobe-CNS1-7.pdf) file that is included in this repository, with 500 glyphs shown per page. And, for reader convenience, the beginning of each Supplement is clearly marked. *Adobe Ming Std L* (aka, AdobeMingStd-Light or Adobe 明體 Std L), designed by Arphic Technology, and owned by Adobe Systems Incorporated. The specific font instance is Version 7.000, as reflected in its /CIDFontVersion dictionary entry.

---
## Changes Since Earlier Versions

The following sections detail the history of this document, which was originally referred to as Adobe Technical Note #5080.

### Since the 2003-05-27—Supplement 4—Version

The glyphs for Supplement 5 (CIDs 18965 through 19087) were added. AdobeMingStd-Light (*Adobe Ming Std L*) with /CIDFontVersion value 5.000 was used for the representative glyphs.

### Since the 2007-02-28—Supplement 5—Version

The glyphs for Supplement 6 (CIDs 19088 through 19155) were added. AdobeMingStd-Light (*Adobe Ming Std L*) with /CIDFontVersion value 6.001 was used for the representative glyphs. The entire document was completely re-written.

### Since the 2012-01-12—Supplement 6—Version

The glyphs for Supplement 7 (CIDs 19156 through 19178) were added. AdobeMingStd-Light (*Adobe Ming Std L*) with /CIDFontVersion value 7.000 was used for the representative glyphs. The entire specification was ported to GitHub markdown syntax and revised.

That is all.
