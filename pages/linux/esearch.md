# esearch 
## chatgpt 
The `esearch` command is a part of the Entrez Direct suite of utilities provided by the National Center for Biotechnology Information (NCBI). It allows users to perform a search of the NCBI's Entrez databases, which include PubMed (biomedical literature), GenBank (genetic sequences), and many others.

The basic syntax of the `esearch` command is as follows:

```
esearch -db [database] -query [search query]
```

Here, `[database]` refers to the name of the Entrez database that you want to search, and `[search query]` is the actual search query you want to perform.

For example, to search the PubMed database for articles related to "cancer treatment", you would use the following command:

```
esearch -db pubmed -query "cancer treatment"
```

When executed, the `esearch` command will return a list of IDs (unique identifiers) for the search results that match your query. You can then use these IDs with other Entrez Direct commands to retrieve more information about the search results, such as the abstracts of PubMed articles or the full genetic sequences of DNA sequences in the GenBank database. 

## tldr 
 
> Perform a new Entrez search using terms in indexed fields.
> It is part of the `edirect` package.
> More information: <https://www.ncbi.nlm.nih.gov/books/NBK179288/>.

- Search the pubmed database for selective serotonin reuptake inhibitor:

`esearch -db pubmed -query "{{selective serotonin reuptake inhibitor}}"`

- Search the protein database using a query and regexp:

`esearch -db {{protein}} -query {{'Escherichia*'}}`

- Search the nucleotide database for sequences whose metadata contain insulin and rodents:

`esearch -db nuccore -query "{{insulin [PROT] AND rodents [ORGN]}}"`

- Display [h]elp:

`esearch -h`
