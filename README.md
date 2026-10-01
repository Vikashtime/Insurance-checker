# A AI insurance checker based on the theme covering home appliances only with easily scalable beyond one theme.
# PS42 Claim Checker

An AI insurance claim checker built with Google Gemini (Vertex AI / Agent Platform) and BigQuery.

## What it does
- Reads a claim message, an optional photo, and a policy PDF
- Decides APPROVE, REJECT or HUMAN CHECK, and names the policy clause it used
- Sends low-confidence claims (under 75%) to a human
- Saves every decision to BigQuery

## Files
- notebook: the backend code (run in Google Colab)
- policy.pdf: the sample insurance policy
- results.txt: real results from a test run
- ps42_claims_screen.html: the review screen

## Not included
Cloud Storage was left out because it needs a billing account.

## How to run
Open the notebook in Colab, add a Gemini API key as a secret called MY_KEY, and run the cells in order.

