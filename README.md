<a href="https://srmek.org/"><img src="media/cover.jpg" alt="SRMEK, home page on a laptop and a phone" width="100%"></a>

# SRMEK

New public site for the Serbian Association for Quality: server-rendered PHP in front of the old Drupal back office.

**[srmek.org](https://srmek.org/)** · [Srpski](README.sr.md)

> [!NOTE]
> Client project. The source code belongs to the client and stays in a private repository. This page describes what I built and how.

<table>
  <tr><td><b>Client</b></td><td>SRMEK</td></tr>
  <tr><td><b>Industry</b></td><td>Quality association: training and resources on management systems</td></tr>
  <tr><td><b>Location</b></td><td>Kragujevac, Serbia</td></tr>
  <tr><td><b>Type</b></td><td>Bilingual multi-page website</td></tr>
  <tr><td><b>My role</b></td><td>Redesign, development, migration, hosting and maintenance</td></tr>
  <tr><td><b>Stack</b></td><td>PHP 8.3, Drupal (back office), Moodle, nginx</td></tr>
</table>

## About the project

SRMEK is the Serbian Association for Quality, based in Kragujevac. It brings together quality managers, auditors, institutions and companies, and runs seminars on ISO 9001, IATF 16949, ISO 14001, ISO 45001 and HACCP. It has also organized an international quality congress and a quality innovation award. I rebuilt its public site in Serbian and English and carried over the news archive, documents and program pages.

I did not move everything at once. The public pages (about 94 URLs in the sitemap) are rendered by PHP 8.3 on the server. Behind them the older Drupal back office still handles forms and files, and Moodle e-learning and the congress systems stay connected. Dated content is labelled as such: program and event pages published years ago carry a note to check dates with the association, and the figures on the home page are marked as coming from the previous site, with no update date.

## What I built

- A server-rendered PHP 8.3 front end with about 94 URLs in the sitemap, in Serbian and English
- The older Drupal back office kept in place behind it for forms and files
- Moodle e-learning and the congress systems connected to the new site
- A training catalogue grouped by area, with seminar codes and length in days
- Notices on outdated program and event pages, and old figures labelled as coming from the previous site
- A strict content security policy with a nonce per request, self-hosted fonts and a button that pauses animations

## Results

| | Performance | Accessibility | Best practices | SEO |
| :-- | :-: | :-: | :-: | :-: |
| Mobile | 100 | 100 | 96 | 100 |
| Desktop | 100 | 100 | 96 | 100 |

Lighthouse, lab test of the live site, September 2026.

## Screenshots

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="SRMEK, home page on a 1440 px screen"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="SRMEK, home page on a phone"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="Training and seminars">
<sub>Training and seminars</sub>

<img src="media/inner-2.webp" alt="Quality and innovation award">
<sub>Quality and innovation award</sub>

---

<sub>Built by [D. Svilenković](https://svilenkovic.com).</sub>
