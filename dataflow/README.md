1)  Go To Cloud Shell
2)  gcloud init
3)  pip install 'apache-beam[gcp]'
4)  python -m attendance \
	--input gs://<your-input-bucket>/csv-files/input/dept_data.txt \
	--output gs://<your-output-bucket>/dflow/output/part \
	--runner DataflowRunner \
	--project <your-project-id> \
	--region <your-region-name> \
	--temp_location gs://<your-output-bucket>/temp/ 
