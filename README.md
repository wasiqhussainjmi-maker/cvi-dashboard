# CVI Finance Dashboard

AP aging dashboard for Castor & Vale Industries, a fictional company. All data is synthetic.

```
Microsoft Fabric (Bronze → Silver → Gold, 1,500+ reconciliation checks)
   └─ nb_cvi_05_publish_to_github  ──commits──▶  public/data/ap_aging.json
                                                    └─ Vercel redeploys ──▶ public dashboard
```

- `public/index.html`: the dashboard. Plain HTML, CSS and SVG, with no libraries.
- `public/data/ap_aging.json`: the data. This file is overwritten by the Fabric publish notebook; don't edit it by hand.
- `vercel.json`: tells Vercel to serve the `public` folder.
