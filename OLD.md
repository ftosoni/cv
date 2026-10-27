# Voci rimosse dal CV

Archivio delle voci tolte da `main.tex` nella revisione di settembre 2026, copiate testualmente dalla versione precedente (commit `9abcbe6`) in modo da poterle reincollare se servono (per esempio in un CV per l'industria). Il file non viene compilato.

## Premi da studente (Arctic Code Vault, HackTheAlps, First Ascent / Bending Spoons)

Erano nella sezione *Awards*, solo nella versione full.

```latex
    \ifshortcv\else% student-era distinctions: full CV only

    \divider

    \cvachievement{\faGithub}{Github --- Arctic Code Vault Contributor}{Awarded Github's Arctic Code Vault Contributor badge as part of the \href{https://archiveprogram.github.com/arctic-vault/}{2020 GitHub Archive Programme}.
    
    This recognition was for the repository \href{https://github.com/ftosoni/Watermark}{\textit{ftosoni/Watermark}}.
    }

    \href{https://github.com/ftosoni/Watermark}{\faLink\ GitHub Repository}

    \divider

    \cvachievement{\faHeartbeat}{HackTheAlps – \#WeAgainstVirus 2020, 3rd Prize}{Awarded 3rd prize for developing the \textit{Pharma-Q} application prototype
    
    \textit{HackTheAlps} focused on proposing software solutions and ideas to support local communities during the \textit{COVID-19} emergency. Our team developed an AI-powered web service to monitor queue lengths at pharmacies in Bozen/Bolzano using data acquired through surveillance cameras.
    }
    
    \href{https://hackthealps.it/weagainstvirus}{\faGlobe\ Event Page} | Team: \href{https://danyele.github.io/}{Daniele Gadler}, \href{https://linkedin.com/in/tj-mustafa-7a423954}{Tajammul Mustafa}, Francesco Tosoni
    
    \divider
    
    \cvachievement{\faTrophy}{First Ascent 2018 Finalist}{Selected from over 400 applicants to participate in \textit{First Ascent 2018}
    
    FA18 (Copenhagen, Denmark) was a coding challenge event organised and sponsored by Bending Spoons. The event brought together 20 top Italian tech students from universities in Italy (Bologna, Cagliari, Padua, Pisa, Rome, Trento), England (Cambridge, Oxford, Imperial College London), and Germany (TUM).
    }
    
    \href{https://firstascent.io}{\faGlobe\ Event Page}

    \fi% end \ifshortcv (student-era distinctions)
```

## Nota sull'articolo IEEE Access [j4]

Frase originale con "principal investigator".

```latex
    As the principal investigator, corresponding and first author, I initiated and led this interdisciplinary research project, bridging theoretical computer science and electronic engineering. My work involved enhancing Google's Zuckerli compressed matrix formats (\href{https://github.com/ftosoni/zuckerli}{Github fork}) to enable computation-friendly matrix-to-vector and PageRank kernel operations. Published as Gold open access under CC~BY~4.0.
```

## Wikimedia Hackathon 2025 e 2026 (versione estesa)

Erano nella sezione *Code artefacts*, ora condensati in "Wikimedia tooling".

```latex
\cvachievement{\faWikipediaW}{Wikimedia Hackathon 2025}{Palermo, Italy | 14--16 Mar 2025}
Contributed to technical enhancements for Wikipedia and sister projects:
\begin{itemize}
    \item \textbf{Automatic spelling detection for Template F}: 
    Optimised a Lombard Wikipedia template to auto-detect article orthography, eliminating manual configuration. \\
    \textit{(Enabled dynamic rendering for regional language variants)}
    
    \item \textbf{Smart image resizing}: 
    Python script leveraging REST APIs to standardise image dimensions across articles, improving page aesthetics. \\
    \textit{(Reduced visual inconsistencies by automated proportional scaling)}
\end{itemize}
\href{https://www.mediawiki.org/wiki/Special:MyLanguage/Wikimedia_Hackathon_2025/Satellite_Events/Palermo}{\faGlobe\ Event Page} %| Team: Super nabla (me), Sciking

\divider

\cvachievement{\faWikipediaW}{Wikimedia Hackathon 2026}{Milan, Italy | 30 Apr--3 May 2026}
Collaborated with the global technical community on infrastructure and semantic tools for MediaWiki:
\begin{itemize}
\item \textbf{MediaWiki Code2Code Search}:
Delivered an unconference session about a semantic search tool using Jina AI embeddings and vector-based retrieval to identify code similarities across the MediaWiki ecosystem. \
\textit{(Enhanced developer navigation and long-term code stewardship via SWH archival)}

\item \textbf{Inclusive UI and Web accessibility} \href{https://github.com/ftosoni/mediawiki-accessibility-checker}{\faGithub}:
Developed and presented a Proof-of-Concept Toolforge tool to test against web accessibility standards like WCAG 2.0 AA.

\end{itemize}
\href{https://www.mediawiki.org/wiki/Special:MyLanguage/Wikimedia_Hackathon_2026}{\faGlobe\ Event Page} %| Team: Super nabla (me), Indic MediaWiki Developers UG

\divider

\begin{itemize}

\item {\bf MediaWiki Accessibility Checker} \href{https://github.com/ftosoni/mediawiki-accessibility-checker}{\faGithub} A proof-of-concept Toolforge tool developed at the Wikimedia Hackathon 2026 that audits MediaWiki pages against web accessibility standards (WCAG 2.0 AA). (\href{https://github.com/ftosoni/mediawiki-accessibility-checker}{GitHub site})

\item {\bf Wikimedia Tool for Translation Tags} \href{https://github.com/indictechcom/translatable-wikitext-converter}{\faGithub} Contributed a web application originally developed by \href{https://github.com/gopavasanth}{Gopa Vasanth} (\href{https://meta.wikimedia.org/wiki/Indic-TechCom}{Indic Wikimedia Technical Committee}) for Wikimedia projects to automate the insertion of translation tags by parsing wikicode. (\href{https://github.com/indictechcom/translatable-wikitext-converter}{GitHub site})

\end{itemize}
```

## Progetti da studente (Watermark, PharmaQ): versioni originali

Con il badge Arctic Code Vault e il 3° posto all'hackathon.

```latex
  \item \textbf{Watermark} \href{https://github.com/ftosoni/Watermark}{\faGithub}\enspace Multi-threaded C++ image-watermarking application (POSIX threads with fork--join, plus a \href{https://github.com/fastflow/fastflow}{FastFlow} version) with performance-evaluation tooling; awarded GitHub's \href{https://archiveprogram.github.com/arctic-vault/}{Arctic Code Vault} Contributor badge (2020 GitHub Archive Programme).
  \item \textbf{We Against Virus~-- PharmaQ} \href{https://github.com/DanyEle/WeAgainstVirus-FTD}{\faGithub}\enspace Flask web portal estimating pharmacy queue lengths from user-submitted photos; 3rd place at the \href{https://hackthealps.it/weagainstvirus}{\#WeAgainstVirus} hackathon.
```

## Sezione progetti (titolo e nota originali)



```latex
\cvsection{Participation in [inter]national projects}

{\em Note}: For each project, I report the associated publications (c1,j1,j2,j3,j4) produced as outcomes.
```

## Visita GRICAD (titolo originale)



```latex
\cvevent{Visiting Researcher}{GRICAD}{25 Nov -- 28 Nov 2025}{Grenoble, France}
```

## Tirocini e stage (sezione completa)

Comprendeva il doppione Inria (luglio 2025), Bending Spoons, EPLASS e Flyeralarm. Bending Spoons, EPLASS e Flyeralarm sono stati poi reintegrati in "Industry experience"; qui resta solo come traccia della versione originale.

```latex
\ifshortcv\else
\cvsection{Professional internships and traineeships}

\cvevent{Research Intern \& Software Development}{Inria --- Software Heritage}{Jul 2025}{Paris, France}
A focused research collaboration on efficient code compression and scalable data retrieval for Software Heritage (Terabyte-scale caching systems and shard-format optimisation), within the CodeCommons project.

\divider

\noindent Earlier internships and traineeships:
\begin{itemize}[leftmargin=1.3em, itemsep=2pt, topsep=1pt, parsep=0pt]
  \item \textbf{Sep 2018}\enspace Invited participant, \textbf{Bending Spoons} (Copenhagen, Denmark) --- selected among 20 top Italian tech students from 400+ applicants for a coding-challenge event.
  \item \textbf{Aug 2014}\enspace Intern, \textbf{EPLASS GmbH} (Würzburg, Germany) --- \texttt{C\#} development at an internet-based software company. {\footnotesize(\href{https://www.francescotosoni.it/static/eplass.pdf}{\faCertificate\,certificate})}
  \item \textbf{Aug 2014}\enspace Intern, \textbf{Flyeralarm GmbH} (Würzburg, Germany) --- cross-departmental operations at a pan-European online printing firm. {\footnotesize(\href{https://www.francescotosoni.it/static/flyeralarm.pdf}{\faCertificate\,certificate})}
\end{itemize}
\fi% end \ifshortcv (Professional internships hidden in the short CV)
```

## Industry experience (sezione completa)

Tolta nella revisione di ottobre 2026: tirocini del 2014 ed evento Bending Spoons del 2018, segnali da studente in un CV accademico post-dottorato.

```latex
\ifshortcv\else
\cvsection{Industry experience}

\begin{itemize}[leftmargin=1.3em, itemsep=2pt, topsep=1pt, parsep=0pt]
  \item \textbf{Sep 2018}\enspace Invited participant, \textbf{Bending Spoons} (Copenhagen, Denmark) --- selected among 20 top Italian tech students from 400+ applicants for a coding-challenge event.
  \item \textbf{Aug 2014}\enspace Intern, \textbf{EPLASS GmbH} (Würzburg, Germany) --- \texttt{C\#} development at an internet-based software company. {\footnotesize(\href{https://www.francescotosoni.it/static/eplass.pdf}{\faCertificate\,certificate})}
  \item \textbf{Aug 2014}\enspace Intern, \textbf{Flyeralarm GmbH} (Würzburg, Germany) --- cross-departmental operations at a pan-European online printing firm. {\footnotesize(\href{https://www.francescotosoni.it/static/flyeralarm.pdf}{\faCertificate\,certificate})}
\end{itemize}
\fi% end \ifshortcv (Professional internships hidden in the short CV)
```

## Voci di Wikipedia avviate (Community Engagement)

Tolta nella revisione di ottobre 2026 dall'inizio della parte `\longonly` della sezione *Open Data Contributions & Community Engagement*.

```latex
\longonly{Initiated 150+ Wikipedia articles; organised Wikimedia Italia meetups
```

## Open Data Contributions & Community Engagement (versione estesa)



```latex
\cvsection{Open Data Contributions \& Community Engagement}

\noindent \textbf{Technical Ecosystem \& Tooling:} Architect and maintainer of open-source tools on Wikimedia Toolforge, including \href{https://code2codesearch.toolforge.org/}{Code2Code Search}, a semantic retrieval engine for the MediaWiki codebase. Developed \href{https://it.wikipedia.org/wiki/Utente:Nablabot}{Nablabot}, an automated framework for cross-wiki data consistency and error correction. Active Videshi member of the \href{https://meta.wikimedia.org/wiki/Indic_MediaWiki_Developers_User_Group}{Indic MediaWiki Developers User Group}, focusing on bulk reconciling data on Wikidata, technical student mentorship (\href{https://diff.wikimedia.org/2026/07/23/indic-wikimedia-hackathon-hyderabad-2026/}{Indic Wikimedia Hackathon Hyderabad 2026}), and large-scale source code preservation and presentation layers.

\vspace{0.5em}

\noindent \textbf{Knowledge Curation \& Impact:} Initiated 150+ articles and curated structured data at scale on Wikidata.

\vspace{0.5em}

\noindent \textbf{Community Leadership \& Outreach:} Frequent collaborator with tech communities, particularly in the Indic region, to foster cross-cultural digitisation. In partnership with \textit{Wikimedia Italia} (WMIT), organised Wikimedian meetups such as \href{https://it.wikipedia.org/wiki/Wikipedia:Raduni/Wiki-cinema_indiano_a_Pisa}{Indian Wiki-cinema} (Pisa, 2025) and \href{https://it.wikipedia.org/wiki/Wikipedia:Raduni/Wiki-Pakistan}{Wiki-Pakistan} (Bolzano, 2024). I contribute technical insights as an \href{https://diff.wikimedia.org/author/super-nabla/}{author on Diff} and served as a jury member for the Wikipedia Asian Month (November 2025).
```
