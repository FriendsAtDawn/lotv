---
Title: "How to deal with infected Judisoft(TM) pdfs."
Description: "Survival guide."
draft: false
date: 2024-02-07
---

Document status: 0.5

It is not my intention to discredit Judisoft(TM) with these brief lines, which even the modest epithet _article_ loosely fits. The implementation of the system is by far the most important leap forward in access to justice and a major contributor to cost reduction. It is a success in every sense of the word.

## Frequency: $$\tfrac{1}{t}$$

It is because I have intensive dealings with all the courts and intensive dealings with only a handful of lawyers that I refer more to documents emanating from the courts than to those filed by colleagues.  It is a question of frequency.

I have never received an infected pdf uploaded by a colleague. In that sense, I don't know. Judisoft(TM) seems to have more control when someone upload a *pdf* from his *front-end*. However, all the files infected was coming from the source.

## Preliminaries.

### Are Judisoft files infected with viruses?

It depends on what you mean by virus. It has suspicious or outright malicious code. But authoritative sites could give little information about it except that it "does something" and definitely takes up space in the traffic.

Folder containing the [original file and *timestamps*](https://bafybeiau7f4waqhoinfba5gci2ecd3hfqxjopoykvfi6cc4sgcmfihyiue.ipfs.nftstorage.link/) It is only there for testing purposes, if you want to open any *pdf*, it is better to open the original, which is at:[https://www.csj.gov.py/verificarDocumento/Default.aspx?c=cdecaech&o=b](https://www.csj.gov.py/verificarDocumento/Default.aspx?c=cdecaech&o=b).

El análisis [hybrid-analisys.com](https://hybrid-analysis.com/sample/d9ceea207e9dd5a0040ca8db12357f4c4a3607520ad993fe057fe84e4f24a25a/65dbb8cb7eaf4029bd001d5a). Note that there are files that are labeled as "legitimate" Adobe resources. And there are others that are not, and there are others that are definitely, I repeat, "legitimate" programs. It's a mixed bag, sometimes difficult to follow, so patience is needed to read all the documents.

### Do they all have it, or even the vast majority?

No, --- in my experience --- very few *pdfs* are infected, given the sheer volume of them. But it is not unreasonable to think that their number is growing. In fact, the file shown here as an example seems to have been duplicated in another file; although it came from a file containing a query of mine, it was attached to another list. As we know very little about how Judisoft(TM) works, this could be another kind of bug.

### Are they dangerous, should I be careful?

There are two answers:

- No. In fact, everyone lives the fantasy that they have nothing to hide from the world - while thinking of their wife.  If this is your case, please leave your ID number and bank password in the message box.

In the other case:

- Yes.

You could be up to no good if nobody knows what these _scripts_ are doing.

### Why is this happening to me?

Well, let's see.

## The PDF/A plan --- Or: I love it when a plan doesn't comes together!

According to the Resolution on the e-Expedient, when we upload a file from our computer, it is re-encoded into PDF/A.

This does not happen.

As far as the judges are concerned, it is impossible to even think of the same process, as it would invalidate the signature.

## The judges were careless?

If I sign a *pdf* (who would think of signing a *pdf*? Someone who came up with the idea that text files are not sexy enough) with my electronic signature, probably not certified, the date is taken from [**Sectigo**](https://sectigo.com). If judges do it, they... they take it from their PC. INTN has an NTP server.

The embedded code is visible to the naked eye, but the Windows antivirus doesn't detect it.

So no. It's not their fault.


## Blocking servers is not the answer.

I don't have the knowledge to know what each one does, but it wouldn't do any good as they change or mutated or whatever.

I can't tell you that the solution is to block *dns* requests. And I don't think everyone has a *dns* server running in their office. And even if they did, what good would it do? These malicious sites mutate every day.

## ¿Y?

I took these emergency steps

- Disable WebRTC: you can do this with an extension that is available for a number of browsers and in a number of flavours.

- Do not allow any *pdf* files to be displayed in the browser.

- Keep the local database out of reach of the internet -- if possible; the internet is everywhere.

I have had infected *pdfs* for printing and scanning. It's the only thing I can do, although I know it's a long shot.

I can't do what some sites recommend:

- Disable Javascript: without JS, Judisoft is not usable and my own database is not usable.

# Is there a political solution?

Yes, but I don't see a future for it. A REST API could be written for people who want to use it to avoid traffic overhead, control access to resources and reduce costs.

There will be no breach of secrecy.

On the contrary, control can be improved.

But... there is a complaint form that is made in ```Google Form```; if there is no time to make a ```<form>```, there will be no time to make an API.

[^1]: And as far as I know, no one has used the Transparency Act to request Judisoft's source code.

{{< graphcomment >}}
