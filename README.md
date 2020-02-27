# DUCAT and CEX

This site is published at <https://eumaeus.github.io/uva_cex_ducat/>.

## What is CEX?



## Some Things You Can Do With CEX

- [Generate a facsimile view of an edited manuscript](https://www.homermultitext.org/facsimiles/venetus-a-2020/pages/urn_cite2_hmt_msA-v1_154v.html)
- [Provide flexible retrieval and searching from a complex dataset via a web-service](http://beta.hpcc.uh.edu/hmt/hmt-microservice/)
- [Generate a reader’s view of a text with syntactic documentation](http://folio2.furman.edu/ot/pages/urn_cts_greekLit_tlg0011_tlg004_1-57.html)
- [Make a lexicon](http://folio2.furman.edu/ot/pages/urn_cts_greekLit_tlg0011_tlg004_1-57.html) or a [dictionary](http://folio2.furman.edu/lewis-short/index.html?urn=urn:cite2:hmt:ls.markdown:n21247)
- [Generate a reader’s view of a text using machine-parsing](https://furman-university-editions.github.io/Readers/Aristotle/Aristotle_Poetics4.html)
- [Provide a dynamic online web-app for browsing and analysis](http://www.homermultitext.org/hmt-digital/index.html?urn=urn:cts:greekLit:tlg0012.tlg001.msA:12.1)


## The Problem of Alignment

- Implicit alignment (prose works) via canonical citation. [Example: John 3.16](https://eumaeus.github.io/uva_cex_ducat/cite-1.15.0.html?urn=urn:cts:greekLit:tlg0031.tlg004.wh_fu:3.16)
- Alignment of Poetry: a hard example.
	- [Greek *Iliad* 5.655-5.667 with Pope’s *Iliad*, Book 5, stanzas 68 and (part of 69)](https://eumaeus.github.io/uva_cex_ducat/ducats/iliad_example.html?urn=urn:cts:greekLit:tlg0012.tlg001.allen:5&urn=urn:cts:fufolio:pope.iliad.fu2019:5.68-5.69.9&urn=)
- Translation Alignment:
	- [Apuleius, *Metamorphosis* 3.16 Latin and (1566) English.](https://eumaeus.github.io/uva_cex_ducat/ducats/apuleius.html?urn=urn:cts:latinLit:phi1212.phi002.gaselee.token:3.16&urn=urn:cts:latinLit:phi1212.phi002.chin.token:3.16&urn=)
	- [Catullus 1](https://eumaeus.github.io/uva_cex_ducat/ducats/catullus_1.html?urn=urn:cts:latinLit:phi0472.phi001.merrill.token:1&urn=urn:cts:latinLit:phi0472.phi001.ozlam.token:1&urn=)
- Alignment of Text to Commentary Text
	- [Weakness of existing UI](https://eumaeus.github.io/uva_cex_ducat/ducats/epictetus.html?urn=urn:cts:greekLit:tlg0557.tlg001.perseus-grc1:1.1-4.12&urn=urn:cts:greekLit:tlg0557.tlg002.perseus-grc1:1-20&urn=)
	- [A better view](https://eumaeus.github.io/uva_cex_ducat/ducats/epictetus.html)
	- [A code notebook might be the better way](https://hub-binder.mybinder.ovh/user/eumaeus-fucite-jupyter-iwl2r94p/notebooks/alignment/sandbox.ipynb). The good stuff is at the bottom! (If asked to set a kernel, choose "Scala 2.12") 

	The DUCAT Tool is merely one method for creating alignments, and merely one way to view them. With an aligned texts, in CEX format, you could, for example, create a [dynamic lexicon](https://hub-binder.mybinder.ovh/user/eumaeus-fucite-jupyter-iwl2r94p/notebooks/alignment/sandbox2.ipynb). The good stuff is at the bottom! (If asked to set a kernel, choose "Scala 2.12")

