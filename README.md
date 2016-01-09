#Wildbow Web Serial Scraper for Kindle

I couldn't find a good ebook/kindle version of worm, the fantastic web serial by wildbow (John McCrae), and subsequent works, so I decided to make one. You can now enjoy worm, pact, and twig without all of the eye strain! Until wildbow gets these things published, this is the next best option.

[Please support the author!](https://parahumans.wordpress.com/support/)

![Worm Header](http://parahumans.files.wordpress.com/2011/06/cityscape2.jpg)

##Download

Download the ebook or run the scraper yourself.

##How to run:

1. Clone this project
2. Install dependencies - Ruby, zlib, and calibre
  
  ```command
  sudo apt-get install ruby-dev
  sudo apt-get install zlib1g-dev
  sudo apt-get install calibre
  ```
  In early versions, uri and open-uri were required gems, but they appear to have been rolled into the Ruby build now. 
  ```command
  gem install nokogiri
  ```
3. Run the script and output into html file

  ```command
  ruby worm_scraper.rb > worm.html
  ```
4. Convert (requires Calibre CLI)

  ```command
  ebook-convert worm.html worm.mobi --authors "John McCrae" --title "Worm" --max-toc-links 500
  ```
