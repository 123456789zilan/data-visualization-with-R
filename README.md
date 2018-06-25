## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/123456789zilan/data-visualization-with-R/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List
# ggplot plot
p2<- ggplot(data=d, aes(x = Petal.Length, y = Petal.Width)) 
p2 + geom_point(aes(color=Species, shape=Species)) 
p2

# box plot
boxplot(d$Petal.Length~Species,data=d, xlab="Species", ylab="Sepal Length", main="Iris Boxplot")

# ggplot box plot
box <- ggplot(data=d, aes(x=Species, y=Sepal.Length))
box + geom_boxplot(aes(fill=Species)) 
ylab("Sepal Length") + ggtitle("Iris Boxplot") 

#histogram 
hist(d$Sepal.Width, breaks=5)

# ggplot histogram 
histogram<- ggplot(data=d, aes(x=Sepal.Width))+xlab("Sepal Width") +  ylab("Frequency") + ggtitle("ggplot Histogram of Sepal Width")
histogram + geom_histogram(binwidth=0.3,color="grey", aes(fill=Species))

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/123456789zilan/data-visualization-with-R/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
