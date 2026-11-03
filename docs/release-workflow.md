# Publishing with GitHub Actions

The manual **Prepare release draft** workflow uses the repository's `GITHUB_TOKEN`, not a personal access token. It creates a draft and reports its creator in the run summary. It does not delete releases, upload packages, publish drafts, or create or move tags. It requires `contents: write` and an existing tag matching `manifest.json`.

## Replacing the existing v1.0.0 release

1. Push the workflow and release notes to `main`. Leave the existing release in place until the workflow is visible in Actions.
2. Retain local copies of both release assets and verify the package against `SHA256SUMS.txt`. Copy any release-note edits you want to keep into `RELEASE_NOTES.md` before running the workflow.
3. Delete only the current **release**, keeping the existing `v1.0.0` **tag**. This removes the old release assets and temporarily breaks their download URLs. Old release comments, reactions, and download counts will not transfer. If GitHub prevents deletion, stop; do not delete or move the tag to work around it.
4. Open **Actions > Prepare release draft > Run workflow**, use branch `main` and tag `v1.0.0`, and leave pre-release off for the approved final release.
5. Check the run summary reports `github-actions[bot]` as the creator. Open its draft link and attach `illustrated-mcat-1.0.0.apkg` and `SHA256SUMS.txt`.
6. Verify the notes and attachments, then publish the draft. Confirm the resulting release attribution before announcing it. Download the asset and compare its SHA-256 with the checksum file.

If manual publication changes the visible attribution, use a separate bot-authenticated publish step after verifying the uploaded assets. This workflow intentionally does not publish an empty release as a workaround.

The existing tag stays on its original commit. The workflow and updated notes are read from the `main` commit used for the workflow run; adding the workflow does not require retagging v1.0.0.

## Identity limits

The release creator, asset uploader, commit author, and workflow initiator are separate identities. A bot-created draft does not anonymize the person running Actions or uploading files. The REST API exposes asset uploader metadata, and workflow history may show the initiating account. Do not promise that this removes every association with a personal account.

Keep Git commit attribution configured as intended. Email association and organization membership visibility are managed separately in GitHub account settings; this workflow does not change them.

References: [workflow permissions](https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax), [release API](https://docs.github.com/en/rest/releases/releases).
