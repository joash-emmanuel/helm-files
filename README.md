create a github repo for your config file


helm create helm --create your config files as required


helm package helm


helm repo index .


push your changes to github


Generate a personal access token


helm repo add frontend-deployment 'https://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@raw.githubusercontent.com/joash-emmanuel/private-frontend-helming/master/'


-- for the above statement (frontend-deployment is the name of our helm repo -- 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 is our personal access token -- joash-emmanuel is the github-username  -- private-frontend-helming is the repo name -- master is the branch name  --dont forget the /branch/' syntax


helm search repo frontend-deployment -- to look for your helm repository

MAKING UPDATES TO YOUR HELM REPOSITORY


Make updates to your config files (dont forget to update the charts.yaml file)


helm package helm


helm repo index --merge index.yaml .


push the changes to github


helm repo update frontend-deployment


helm search repo frontend-deployment

helm repo list ---- to get the name of the helm repo and url
