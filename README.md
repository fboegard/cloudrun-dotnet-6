# .NET 6 on Google Cloud Run

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)

.NET 6 was [released](https://devblogs.microsoft.com/dotnet/announcing-net-6/) on November 8, 2021 and is a LTS release, supported for three years.

## Deploy to Cloud Run

[Cloud Run](https://cloud.run) allows you to run your .NET app in a fully managed serverless environment.

To deploy to Cloud Run, use the button above, or the following steps:

* Build with `gcloud builds submit --tag gcr.io/$PROJECT_ID/dotnet6`
* Deploy with `gcloud run deploy --image gcr.io/$PROJECT_ID/dotnet6`

Replacing `$PROJECT_ID` with your Google Cloud project ID.

## Running locally

* Build with `docker build -t dotnet6 .`
* Start with `docker run -p 8080:8080 dotnet6`
* Open in your browser at `http://localhost:8080`