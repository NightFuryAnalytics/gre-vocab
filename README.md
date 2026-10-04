# GRE Vocabulary

A simple, mobile-friendly vocabulary app for reviewing GRE words on the go.

**[Open the app](https://NightFuryAnalytics.github.io/gre-vocab/)** once GitHub Pages is enabled.

## What’s included

- **878 words and phrases**, grouped into eight sections of 100 and a final section of 78.
- Tap any word to see its meaning, example sentence, English and Roman Urdu mnemonics, synonyms, and antonyms.
- Source tags: **160+**, **High frequency**, **Confusing words**, and **New words 2023**. Detail cards include the original set numbers where applicable.
- Category filter chips: select one or more categories, or choose **All words** to reset.
- Search across sections, including supported word forms from the source PDF.
- **✓ Mark as read** on each detail card. Tap again to mark it unread. Read words also show a checkmark in lists and search results.
- Next/Previous navigation stays within the selected categories.

## Use the app

1. Choose your categories on the sections page, or leave **All words** selected.
2. Open a section and tap a word.
3. Review the card and mark it as read when ready.
4. Continue with **Next word**, or return to the word list.

Filters and read checkmarks are saved in your browser’s local storage. They do not sync between devices or browsers. Clearing site data removes them. The downloaded file and the hosted website have separate storage.

## Run locally

Open `index.html` in a modern browser. No installation, build step, account, or API key is needed.

The HTML file contains the app’s content, styles, and scripts. A downloaded copy can be used offline; external dictionary links require internet. Reading and basic navigation also work without JavaScript, but search, filters, and read tracking require it.

Opening the hosted website does not automatically install an offline copy.

## Publish with GitHub Pages

After pushing this repository to GitHub:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose **main** and **/ (root)**, then click **Save**.
4. Once deployment completes, visit <https://NightFuryAnalytics.github.io/gre-vocab/>.

See [GitHub’s publishing-source instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Publish an updated app

In the original workspace layout, run these commands from the `github-site` folder after regenerating `outputs/GRE-Vocabulary.html`:

```bash
cp ../outputs/GRE-Vocabulary.html index.html
git add index.html README.md .nojekyll
git commit -m "Update GRE vocabulary app"
git push origin main
```

If you cloned only this repository, edit or replace `index.html` directly, then commit and push. GitHub Pages publishes subsequent changes to the configured branch automatically.

## Content notes

The vocabulary was adapted from the supplied **GRE-341-LIST-NEW.pdf**. Repeated entries were merged, and inflected verbs generally appear under their base forms. Meanings were reviewed and rewritten, with targeted dictionary checks for questionable definitions. Dictionary links appear under **About these words** in the app.

The **160+** tag reflects the PDF’s hard-section lists, not an independently verified difficulty rating or a score guarantee. The separately headed **New Words 2023** list has its own tag. Words can belong to more than one source list.

Definitions cover selected study senses rather than every dictionary sense. Synonyms and antonyms depend on context; contextual contrasts are labeled. Mnemonics are memory associations, not etymological claims. Roman Urdu spelling may vary.

**Review status:** study material is a draft for user review. Marking a word as read records that you reviewed it; it does not certify mastery.

## Repository files

| File | Purpose |
| --- | --- |
| `index.html` | Complete standalone vocabulary app |
| `.nojekyll` | Serves the site without Jekyll processing |
| `README.md` | Usage and deployment instructions |

No analytics, trackers, or backend are included.
