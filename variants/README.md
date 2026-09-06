# Variants

Three versions of the one-page portfolio, same design (bordeaux/white, Newsreader + IBM Plex Mono), different content.

- `christian-cs/` – copy of the live site (Technical Computer Science), kept as an extra.
- `econometrics/` – template for an Econometrics & Operations Research student.
- `math-econometrics/` – template for a Mathematics + Econometrics double-degree student.

Each folder is self-contained: copy it into its own repo and it works as-is.

## Filling in a template

Search the file for `[` and replace every bracketed placeholder: name, city, university, email,
GitHub/LinkedIn usernames, project links, experience, grades. The example projects are plausible
but invented, so swap them for real ones. Add photos to an `img/` folder and replace the two
dashed `.thumb` boxes in "Fun stuff" with an `<img>` like in `christian-cs/index.html`.

Accent colour is one variable: `--wine` in the `:root` block at the top of the file.

## Background figure in `math-econometrics/`

The scroll-driven figure there is not the Lorenz attractor used on the other pages but the
closed loop of a Guéant–Lehalle–Fernandez-Tapia market maker quoting around a Stoikov
micro-price, state (q, I, D), with a weak periodic component in the order flow.
24 slices in τ (the micro-price lag) are precomputed at load with RK4; scrolling cross-fades
between neighbouring slices and rotates the projection. Notes on the choices that differ from
the original brief are in the comment block at the top of the script in `index.html`.
