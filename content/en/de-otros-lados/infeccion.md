---
Title: "How to deal with infected Judisoft(TM) pdfs."
Description: "Survival guide."
draft: true
date: 2024-02-07
---

Document status: 0.5

It is not my intention to discredit Judisoft(TM) with these brief lines, which even the modest epithet _article_ loosely fits. The implementation of the system is by far the most important leap forward in access to justice and a major contributor to cost reduction. It is a success in every sense of the word.

## Frequency: $$\tfrac{1}{t}$$

It is because I have intensive dealings with all the courts and intensive dealings with only a handful of lawyers that I refer more to documents emanating from the courts than to those filed by colleagues.  It is a question of frequency.

I have never received an infected pdf uploaded by a colleague. In that sense, I don't know. Judisoft(TM) seems to have more control.

## Preliminaries.

### Are Judisoft files infected with viruses?

It depends on what you mean by virus. It has suspicious or outright malicious code. But both I and more authoritative sites could give little information about it except that it "does something" and definitely takes up space in the traffic.

TODO: I will copy an example below. There will be a link for the pdf and it's sums, you won't want to check it yourself. Instead, you will check the corresponding link from the analysis page.

### Do they all have it, or even the vast majority?

No, --- in my experience --- very few ```pdfs``` are infected, given the sheer volume of them. But it is not unreasonable to think that their number is growing. In fact, the file shown here as an example seems to have been duplicated in another file; although it came from a file containing a query of mine, it was attached to another list. As we know very little about how Judisoft(TM) works, this could be another kind of bug.

### Are they dangerous, should I be careful?

There are two answers:

- No. In fact, everyone lives the fantasy that they have nothing to hide from the world - while thinking of their wife.  If this is your case, please leave your ID number and bank password in the message box.

In the other case:

- Yes.

You could be up to no good if nobody knows what these _scripts_ are doing.

### Why is this happening to me?

Well, let's see.

## The PDF/A plan --- Or: I love it when a plan comes together!

According to the Resolution on the e-Expedient, when we upload a file from our computer, it is re-encoded into PDF/A.

This does not happen.

As far as the judges are concerned, it is impossible to even think of the same process, as it would invalidate the signature.

## The judges were careless?

If I sign a ```pdf``` (who would think of signing a ```pdf```? Someone who came up with the idea that text files are not sexy enough) with my electronic signature, probably not certified, the date is taken from [```Sectigo```](https://sectigo.com). If judges do it, they... they take it from their PC. INTN has an NTP server.

The embedded code is visible to the naked eye, but the Windows antivirus doesn't detect it.

So no. It's not their fault.

## My whispered sorrowed talk.

But I'm safe from them. I've had problems with Paperless-ngx detecting them. I don't use very popular systems, and the codes I've seen so far are for the Windows environment.

Nevertheless, I decided to remove them from my archive, because it is very easy for someone in their daily life to send some "SD" via email and infect someone else's PC that way.

At least that's what I thought. That I was safe. But today I checked the ```dns``` traffic in the office... and no, my pdfs have been ```calling home``` for a while, it's just that after one site made too many requests and downloaded about 1Gb of I don't know what, the server blocked that traffic and sent me a message. The kind I never read.

## Blocking servers is not the answer.

I don't have the knowledge to know what each one does, but it wouldn't do any good as I've already identified about 5 different ones. Bah. I didn't recognise it. I hi

I can't tell you that the solution is to block ```dns``` requests. And I don't think everyone has a ```dns``` server running in their office. And even if they did, what good would it do? These malicious sites mutate every day.

## ¿Y?

I took these emergency steps

- Disable WebRTC: you can do this with an extension that is available for a number of browsers and in a number of flavours.

- Do not allow any ```pdf``` files to be displayed in the browser.

- Keep the local database out of reach of the internet -- if possible; the internet is everywhere.

I have had infected ```pdfs`` for printing and scanning. It's the only thing I can do, although I know it's a long shot.

I can't do what some sites recommend:

- Disable Javascript: without JS, Judisoft is not usable and my own database is not usable.

# Is there a political solution?

Yes, but I don't see a future for it. A REST API could be written for people who want to use it to avoid traffic overhead, control access to resources and reduce costs.

There will be no breach of secrecy.

On the contrary, control can be improved.

But... there is a complaint form that is made in ```Google Form```; if there is no time to make a ```<form>```, there will be no time to make an API.

[^1]: And as far as I know, no one has used the Transparency Act to request Judisoft's source code.

{{< graphcomment >}}
