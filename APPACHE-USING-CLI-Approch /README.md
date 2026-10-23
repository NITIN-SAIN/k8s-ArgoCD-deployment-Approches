# create Application using CLI Approach . 

argocd app create apache-app \
  --repo https://github.com/<your-username>/argocd-demos.git \
  --path cli_approach/apache \
  --dest-server https://<your_added_cluster_url> \
  --dest-namespace default \
  --sync-policy automated \
  --self-heal \
  --auto-prune
