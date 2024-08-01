---
title: Topological order on a torus
summary: "The Fractional Quantum Hall effect revealed new phases of matter beyond traditional paradigms, characterized by ground state degeneracy, nontrivial particle statistics, and gapless edge excitations, making them promising for fault-tolerant quantum computation. Determining the topological phase from a microscopic Hamiltonian is challenging, as it often assumes the ground state contains all topological information. It is proposed that topological data can be extract from ground-state wavefunction overlaps, however, this method was impractical for lattice systems. This issue was addressed by constructing specific operators and managing phase factors, applying Wen's results to lattice systems."
tags:
  - Topological order
#date: '2022-04-27T00:00:00Z'
show_date: false

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Calculating the overlap between two states
  focal_point: Smart

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

After the discovery of the Fractional Quantum Hall eﬀect, more and more bizarre phases of matter that cannot be described by the Landau-Ginzburg symmetry-breaking paradigm were found. Instead of normal order parameters, these phases are characterized by robust ground state degeneracy, nontrivial particle statistics, and gapless edge excitations. These properties are robust to small Hamiltonian deformations, making them a potential candidate for fault-tolerant quantum computation.


While multiple exact solvable microscopic Hamiltonians realize the nontrivial topological phase, the inverse problem—i.e., determining the topological phase from the microscopic Hamiltonian—is extremely challenging. Many existing methods are based on the belief that the ground state alone encodes all the information regarding the topological order. A well-known example is that: on a torus, the ground state degeneracy equals the kinds of point-wise excitation of the system.



To extract more information from ground states, we can take other operations, such as the overlap of states. Xiaogang Wen first proposes obtaining the topological data from the overlap of ground-state wavefunctions. However, his argument relies on a continuous deformation in the moduli space (i.e., torus geometry) and is rather impractical to implement in a lattice system. 


We addressed this issue by explicitly constructing operators associated with the physical process and carefully keeping track of the unnecessary phases related to physical/lattice systems. By consistently arranging the phases along every simple loop on the torus, we successfully justified Wen's results in a lattice system.