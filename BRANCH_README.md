# Website Development

This package is intended for a new `website-development` branch of the existing repository.

## Improvements
- Refined landing page and navigation
- Clear notebook explorer
- Browser-based multi-domain simulator for mechanical, RLC electrical, pneumatic and hydraulic models
- Control-methods showcase
- Pole-zero and Bode visualizations
- MATLAB/Simulink comparison
- Responsive layout
- GitHub Pages compatible

## Branch workflow
```bash
git checkout master
git pull
git checkout -b website-development
```

Replace the existing `docs/` contents with the `docs/` folder from this package, then:

```bash
git add docs
git commit -m "Develop multi-domain interactive project website"
git push -u origin website-development
```

GitHub Pages can remain on `master/docs` while this branch is developed. Merge into `master` only after review.
