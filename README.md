# Zusammenfassung der Analysis für das Gymnasium in Bayern PuLSt 12
### Paket onepgnote wurde so verändert, dass subsection und subsubsection farbig hinterlegt werden
### Renewcommand

``` 
\renewcommand{\subsection}[1]{%
	\par\noindent
	\tcbox[colback=red!10!white,
	       colframe=cyan!40!black,
	       boxrule=0.4pt,
	       sharp corners,
	       left=2pt, right=2pt, top=1pt, bottom=1pt,
	       nobeforeafter,
	       box align=base,
	       width= \linewidth]{%
		\bfseries #1%
	}%
}
 \renewcommand{\subsubsection}[1]{%
	\par\noindent
	\tcbox[colback=yellow!20!white,
	       colframe=gray!50,
	       boxrule=0.3pt,
	       sharp corners,
	       left=2pt, right=2pt, top=1pt, bottom=1pt,
	       nobeforeafter,
	       box align=base,
	       width=\linewidth]{%
		\bfseries #1%
	}%
}

### ToDo funktioniert, allerdings nur in der inline Variante nutzbar da kein Platz am Rand des Dokuments

### 