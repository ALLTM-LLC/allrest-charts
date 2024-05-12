# allrest-charts
To update the helm chart repository, run the following commands:

```bash
 ~/projects/allrest-charts/charts/allsupplier-api/ [main] helm package .   
 ~/projects/allrest-charts/charts/allsupplier-api/ [main] helm repo index . --url http	s://alltm-llc.github.io/allrest-charts/charts/
```
This will create a new version of the chart and update the index.yaml file.

Copy the content of the index.yaml file to the index.yaml file in the root of the repository.  
'git add .' and 'git commit -m "Update index.yaml"' and 'git push' to update the repository.  
This will trigger the GitHub Pages action to update the repository.  
