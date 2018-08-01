# Teresa Carreño Performance Data

This is a dataset of repertoire performed by Teresa Carreño in concerts during the years 1863 through 1917. It is not comprehensive, but represents data that has been culled during my research from concert programs and in a few cases, indexes, held at various institutions and archives around the world.

All data associated with each composition is structured as a row so that the fields can be searched in relation to other fields, such as decade, date, venue, etc. The data is presented in CSV and XML formats in order to enable re-use and further research.

The following column headings are used in the CSV spreadsheet:

| Decade | Date | Venue | City | State | Country | Coverage | 

| Composer Name | Variant Title | Work Title | Concert Info | Works Info | Conductor/Performer |

| Holdings 1 | RISM Sigla 1 | Holdings 2 | RISM Sigla 2 | Resource URL | Record URL |

The XML is structured this way:

``` 
<performances>
    <performance>
            <Location>
                <city/>
                <state/>
                <country/>
                <coverage/>
            </Location>
            <Venue/>
            <Decade/>
            <Date/>
            <Notes/> <!-- in data this is equivalent to Concert Info -->
        <worksInfo>
            <work>
                <composerName/>
                <workTitle>
                    <variantTitle/>
                </workTitle>/>
                <artistName/>  <!-- in data this is equal to Conductor/Performer, included only if there are listed performers or conductors -->
                <ensemble/>
                <Notes/> <!-- in data this is equal to Works Info -->
            </work>
        </worksInfo>
        <programInfo>
            <holdingsInfo>
                <Holdings1/>
                <RISM1/>
                <Holdings2/>
                <RISM2/>
            </holdingsInfo>
            <idno>
                <resource>
                <record/>
            </idno>
        </programInfo>
    </performance>
</performances>
```

This dataset is shared under a CC0 1.0 Universal license. If you use this dataset in your work, please acknowledge and attribute appropriately.


