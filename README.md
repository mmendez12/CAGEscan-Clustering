# CAGEscan clustering tools

    Copyright: 2011-2013 RIKEN Omics Science Center
                  2013   RIKEN Center for Life Science Technologies, Division of Genomics Technologies
    Author: Nicolas Bertin <nbertin@gsc.riken.jp>
    License: GNU public license version 2 (GPL v2)

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

This work was supported by a research grant from the Japanese Ministry of
Education, Culture, Sports, Science and Technology (MEXT) for the RIKEN Omics
Science Center to Yoshihide Hayashizaki, and by a research grant from MEXT
to the RIKEN Center for Life Science Technologies.

## CAGEscan-Clustering

Create CAGEscan clusters from paired-end data in BED12, BAM or SAM format,
using the data itself as a guide or an optional list of CAGE Tag Starting Site
(CTSS) clusters in BED6 format.

CAGEscan-Clustering is a Perl script written at RIKEN, that calls
`pairedBamToBed12` and other programs from the BEDTools suite.  It is fully
documented in the file [CAGEscan-Clustering.pod](CAGEscan-Clustering.pod).

## See also

 * http://fantom.gsc.riken.jp/protocols/nanocage.html
 * http://fantom.gsc.riken.jp/software/
 * Linking promoters to functional transcripts in small samples with nanoCAGE and CAGEscan.
   Plessy, Bertin, Takahashi, Simone et al., Nat Methods. 2010 Jul;7(7):528-34.
   http://dx.doi.org/10.1038/nmeth.1470
 * Definition of Promotome–Transcriptome Architecture Using CAGEscan
   Bertin et al., 2012.  Chapter 3 of "Tag-Based Next Generation Sequencing", Wiley-VCH Verlag GmbH & Co. KGaA
   http://dx.doi.org/10.1002/9783527644582.ch3
 * Digital expression profiling of the compartmentalized translatome of Purkinje neurons.
   Kratz, Beguin et al., Genome Res. 2014 (in press).
   http://dx.doi.org/10.1101/gr.164095.113

## pairedBamToBed12

Converts 'properly paired' BAM alignments to BED12 format, to ease the display
and analysis of CAGEscan data.

The source of pairedBamToBed12 is distributed as a patched version of BEDTools:

    https://github.com/nicolas-bertin/bedtools-pairedBamToBed12
