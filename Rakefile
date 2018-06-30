require_relative './config/environment'

def reload!
  load_all './lib'
end

task :console do
  Pry.start
end

task :scrape_rooms do
  # instantiate a scraper, and have it find new rooms
  # would normally start writing tests to define this functionality
  nyc_scraper = RoomScraper.new('https://newyork.craigslist.org/search/roo')
  nyc_scraper.call
  portland_scraper = RoomScraper.new('https://portland.craigslist.org/search/roo')
  portland_scraper.call
  # after this method, should be able to call Room.all and have rooms there
end
