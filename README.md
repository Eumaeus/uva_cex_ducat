# DUCAT and CEX

This site is published at <https://eumaeus.github.io/uva_cex_ducat/>.

## What is CEX?

[The Spec.](https://cite-architecture.github.io/citedx/CEX-spec-3.0.2/) 

[The API for a Scala library.](https://cite-architecture.github.io/cite-api-docs/cex/api/edu/holycross/shot/cex/index.html)

CEX, the CITE Exchange Format, is a plain-text, self-describing format for serializing data from a CITE library: texts, collections, data-models, and indices. It is equally useful for small data and very large data. The [CITE Architecture](http://cite-architecture.org) includes [(very well tested) code](https://cite-architecture.github.io/cite-api-docs/) for ingesting CEX, among other things.

## What About TEI?

CEX is a complement to TEI-XML. It should be entirely possible to move data back and forth between the two formats. TEI users might be interested in [Thomas Köntges’ TEItoCEX tool.](https://github.com/ThomasK81/TEItoCEX)

## Some Things You Can Do With CEX

- [Generate a facsimile view of an edited manuscript](https://www.homermultitext.org/facsimiles/venetus-a-2020/pages/urn_cite2_hmt_msA-v1_154v.html)
- [Allow you to document regions-of-interest on an image](http://www.homermultitext.org/ict2/index.html?urn=urn:cite2:hmt:vaimg.2017a:VA154VN_0656@0.2469,0.3351,0.2181,0.09820&urn=urn:cite2:hmt:vaimg.2017a:VA154VN_0656@0.2522,0.4307,0.2181,0.2976)
- [Provide flexible retrieval and searching from a complex dataset via a web-service](http://beta.hpcc.uh.edu/hmt/hmt-microservice/)
- [Generate a reader’s view of a text with syntactic documentation](http://folio2.furman.edu/ot/pages/urn_cts_greekLit_tlg0011_tlg004_1-57.html)
- [Make a lexicon](http://folio2.furman.edu/ot/pages/urn_cts_greekLit_tlg0011_tlg004_1-57.html) or a [dictionary](http://folio2.furman.edu/lewis-short/index.html?urn=urn:cite2:hmt:ls.markdown:n21247)
- [Generate a reader’s view of a text using machine-parsing](https://furman-university-editions.github.io/Readers/Aristotle/Aristotle_Poetics4.html)
- [Provide a dynamic online web-app for browsing and analysis](http://www.homermultitext.org/hmt-digital/index.html?urn=urn:cts:greekLit:tlg0012.tlg001.msA:12.1)


## Alignment, CEX, and DUCAT

[DUCAT](https://github.com/Eumaeus/ducat), the “Daughter of Ugarit Citation Alignment Tool” is a “single-page webapp” (that is, no back-end, just double-click the `.html` file and start working) that uses CEX to do *citation* alignment. 

DUCAT is inspired by, and a follow-up to, [Ugarit](http://ugarit.ialigner.com), the citation-alignment tool created by Maryam Foradi, Chiara Palladino, and Tariq Yousef at the University of Leipzig. Ugarit had specific goals. DUCAT’s are different.

- Implicit alignment (prose works) via canonical citation. [Example: John 3.16](https://eumaeus.github.io/uva_cex_ducat/cite-1.15.0.html?urn=urn:cts:greekLit:tlg0031.tlg004.wh_fu:3.16)
- Alignment of Poetry: a hard example.
	- [Greek *Iliad* 5.655-5.667 with Pope’s *Iliad*, Book 5, stanzas 68 and (part of 69)](https://eumaeus.github.io/uva_cex_ducat/ducats/iliad_example.html?urn=urn:cts:greekLit:tlg0012.tlg001.allen:5&urn=urn:cts:fufolio:pope.iliad.fu2019:5.68-5.69.9&urn=)
- Translation Alignment:
	- [Apuleius, *Metamorphosis* 3.16 Latin and (1566) English.](https://eumaeus.github.io/uva_cex_ducat/ducats/apuleius.html?urn=urn:cts:latinLit:phi1212.phi002.gaselee.token:3.16&urn=urn:cts:latinLit:phi1212.phi002.chin.token:3.16&urn=)
	- [Catullus 1](https://eumaeus.github.io/uva_cex_ducat/ducats/catullus_1.html?urn=urn:cts:latinLit:phi0472.phi001.merrill.token:1&urn=urn:cts:latinLit:phi0472.phi001.ozlam.token:1&urn=)
- Alignment of Text to Commentary Text
	- [Weakness of existing UI](https://eumaeus.github.io/uva_cex_ducat/ducats/epictetus.html?urn=urn:cts:greekLit:tlg0557.tlg001.perseus-grc1:1.1-4.12&urn=urn:cts:greekLit:tlg0557.tlg002.perseus-grc1:1-20&urn=)
	- [A better view](https://eumaeus.github.io/uva_cex_ducat/ducats/epictetus.html?urn=urn:cts:greekLit:tlg0557.tlg001.perseus-grc1:1.29.41&urn=urn:cts:greekLit:tlg0557.tlg001.perseus-grc1:4.7.13&urn=urn:cts:greekLit:tlg0557.tlg002.perseus-grc1:17.1&urn=)
	- [A code notebook might be the better way to interact with an alignment of the *Epitome* and the *Encheiridion*](https://hub.gke.mybinder.org/user/eumaeus-fucite-jupyter-gtlzgm4v/notebooks/alignment/sandbox.ipynb). The good stuff is at the bottom. (If asked to set a kernel, choose "Scala 2.12") 

	The DUCAT Tool is merely one method for creating alignments, and merely one way to view them. With an aligned texts, in CEX format, you could, for example, create a [dynamic lexicon from a translation-alignment of Catullus](https://hub.gke.mybinder.org/user/eumaeus-fucite-jupyter-gtlzgm4v/notebooks/alignment/sandbox2.ipynb). The good stuff is at the bottom! (If asked to set a kernel, choose "Scala 2.12") There are [other code notebooks using CITE](https://github.com/Eumaeus/fuCite-jupyter) that can be launched via the **launch binder** button.

