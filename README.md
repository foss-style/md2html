# md2html
As we do a lot of written development using md in GitHub*, we do need to place the final copy in HTML or a CMS - a viewer and converter will be useful to save time and be more efficient and error free.

Using Sphinx with recommonmark, we are able to convert md to html using a python based tool.
Using Jekyll requires ruby.

## Install recommonmark

    pip3 install recommonmark

or

    pip install recommonmark

Then, change the conf.py for Sphinx -

### add: 

    import recommonmark

### then

    from recommonmark.parser import CommonMarkParser
    source_parsers = {

    '.md': 'recommonmark.parser.CommonMarkParser',
    }   


