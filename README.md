# Juncture, initial version

The [Plant Humanities Lab](https://lab.plant-humanities.org) is a web site hosting visual essays that "Explore the cultural histories of plants and their influence on human societies".  The Plant Humanities Lab was launched in 2021 as a key output of 2 Mellon funded projects jointly conducted by Dumbarton Oaks and JSTOR Labs.

The infrastructure for the Plant Humanities Lab enables non-programmers to generate a single visual essay or a rich web site consisting of multiple interactive visual essays.

A generalized version of the visual essay rendering code developed for the Plant Humanities Lab was released at the conclusion of the development projects as [Juncture](https://juncture-digital.org)

## What is Juncture exactly?

In simplest terms, Juncture is a Markdown rendering engine that understands how to interpret and render a few special tags to create interactive viewers.

Juncture also provides a few optional companion services

- IIIF services for dynamic rendering of high-resolution images when IIIF versions of an image are not provided by an image provider
- A semantic search tool for locating images and documents for use in visual essay development
- A web-based authoring environment

## Viewing a Juncture essay

Any Markdown file in Github can be used a Juncture visual essay.  All that is needed is to point the Juncture rendering engine to the file.

> [https://juncture-digital.org](https://juncture-digital.org) + `Github username` + `Github repository name` + `Optional repository file path`

For example, 

- to render this file as a Juncture visual essay - [https://juncture-digital.org/rsnyder/uva-demo](https://juncture-digital.org/rsnyder/uva-demo)
- to render a demo file in this repository - [https://juncture-digital.org/rsnyder/uva-demo/demo/amalfi-coast](https://juncture-digital.org/rsnyder/uva-demo/demo/amalfi-coast)

## Key technologies used in Juncture

A guiding principle in the development of the Plant Humanities Lab (and the subsequent evolution of Juncture) was use of free and/or open-source tools where possible in a minimal computing environment. 

### Github

[GitHub](https://www.github.com), Inc. is a platform and cloud-based service commonly used for software development and version control.  It provides distributed version control plus access control, bug tracking, software feature requests, task management, continuous integration, and project wikis.  Github has been a subsidiary of Microsoft since 2018.

As of January 2023, GitHub reported having over 100 million developers and more than 372 million repositories, including at least 28 million public repositories. It is the world's largest source code host as of June 2023.

Github features incclude,

- File storage (Markdown, images, annotations, etc)
- Version control
- Support for implementation of publishing workflows
- Web hosting, with custom domains
- Most features are free to use (including all features used by Juncture)

### Markdown

[Markdown](https://www.markdownguide.org/) is a lightweight markup language for creating formatted text using a plain-text editor. Markdown was created in 2004 as a markup language that is easy to read in its source code form.  Markdown is widely used for blogging and instant messaging, and also used elsewhere in online forums, collaborative software, documentation pages, and readme files.

### Wikidata

[Wikidata](https://www.wikidata.org) is a collaboratively edited multilingual knowledge graph hosted by the Wikimedia Foundation.It is a common source of open data that Wikimedia projects such as Wikipedia, and anyone else, can use under the CC0 public domain license. Wikidata is a wiki powered by the software MediaWiki, including its extension for semi-structured data, the Wikibase.

### International Image Interoperability Framework (IIIF)

[The International Image Interoperability Framework](https://iiif.io) (IIIF, spoken as 'triple-I-eff') defines several application programming interfaces that provide a standardised method of describing and delivering images over the web, as well as "presentation based metadata" (that is, structural metadata) about structured sequences of images. If institutions holding artworks, books, newspapers, manuscripts, maps, scrolls, single sheet collections, and archival materials provide IIIF endpoints for their content, any IIIF-compliant viewer or application can consume and display both the images and their structural and presentation metadata.

### Leaflet

[Leaflet](https://leafletjs.com/) is an open source JavaScript library used to build web mapping applications. First released in 2011, it supports most mobile and desktop platforms, supporting HTML5 and CSS3. Among its users are FourSquare, Pinterest and Flickr.

Leaflet allows developers without a GIS background to very easily display tiled web maps hosted on a public server, with optional tiled overlays. It can load feature data from GeoJSON files, style it and create interactive layers, such as markers with popups when clicked.

### GeoJSON

[GeoJSON](https://geojson.org/) is an open standard format designed for representing simple geographical features, along with their non-spatial attributes. It is based on the JSON format.

The features include points (addresses and locations), line strings (streets, highways and boundaries), polygons (countries, provinces, tracts of land), and multi-part collections of these types.

# Juncture, version 2

Following the release of Juncture in Fall 2021, a next-gen version was developed to address some of the lessons learned in developing and using the first version.

- Improved flexibility in page layouts, including better rendering on mobile devices
- Enhanced IIIF support, including new capabilities for creating and using self-hosted image collections in Github
- Authoring tools for easier editing
    - Preview from editor
    - Drag-and-drop for images and videos with automatic tag creation
- Improved on-line documentation with drag-and-drop and cut-paste code snippets
- Viewer components reimplemented as standard HTML5 Web Components enabling use outside of Juncture environments, including in vanilla HTML pages and Wordpress

# Resource finder (aka, semantic search tool)

The Plant Humanities Lab release in 2021 was accompanied with a search tool for finding images and journal articles, and presenting data extracted from the Wikidata knowledge graph.  The tool was at an alpha level of completeness and quality but showed much promise.

An updated version of the tool is currently under development with completion expected by the end of the year.  An in-process version of the tool can seen at [https://search.plant-humanities.org](https://search.plant-humanities.org).

Improvements in this next version of the tool (will) include:

- Simplified user interface
- On-the-fly generation of IIIF manifests for images
- Support for Juncture drag-and-drop viewer tagging in Juncture editor
- Selecting and saving favorites
- Crowd sourced entity tagging
- Easier addition of new resource providers
- Federated image and document searching with endless-scroll viewing
- More options for filtering and sorting

# Examples

## Some sites currently using Juncture

- [Kent Maps Online](https://www.kent-maps.online)
- [Biodiversity Stories](https://www.juncture-digital.org/Digital-Scholarship-NUS-Libraries/biodiversitystories/) - Site developed by Katherine Enright, a participant in a Dumbarton Oaks summer program
- [Edison Papers Exhibit Site](https://www.juncture-digital.org/edisonpapers/Latimer)
- [DigitalPeni](https://digitalpeni.org/)
- [University of Colorado](https://da4asandbox.github.io/modules/historicizing-data/)
- [Print & Probability](http://bookhistory.rocks/)

## Demo essays

- [Juncture V2](demo/amalfi-coast)
- [Juncture V1](demo/amalfi-coast-j1)
- [Plain HTML](https://rsnyder.github.io/uva-demo/demo/amalfi-coast-html)

# For more info...

Contact me at:

- [https://github.com/rsnyder](https://github.com/rsnyder)
- Ron.Snyder@ITHAKA.org
