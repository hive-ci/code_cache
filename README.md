# code_cache
Version control checkout abstraction and cache.

## Usage

    repo =  CodeCache.repo( repo_url )
    begin
      repo.checkout( :head, 'path/to/checkout' )
    rescue => e
      puts "Checkout failed"
    end

## Testing

Tests run against the github svn and git endpoints for this repository. Just run:

    bundle
    bundle exec rspec
    
