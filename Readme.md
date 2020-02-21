# React Coding Challenge
Frontend coding challenge task including React and test setup
## Description
You will be creating a React application which shows our awesome content. The feature demanded by the users is to see most popular content. The UX and Design team came up with the final design and the Product Owner wants you to implement a `HeroLane` component rendering 3 most popular movies including the background image, title, description and some meta information. We will use the MovieDB as a mocked database for content and [create-react-app](https://create-react-app.dev/docs/getting-started/) as an initial setup.
## User Story
As an **user**, **I want** to see popular movies inside a lane **in order** to discover more content.
## Technical Details
**1. Fetch movies from MovieDB**
You will need to fetch the first 3 most popular movies from the MovieDB with its background images. You can use the API Key for the requests given below. You will also find further links to receive data and images.
| Description           | Value                                                |
| --------------------- | ---------------------------------------------------- |
| API Key               | bce2bca3c8a838c2a1176df5c0246f51                     |
| Get Popular Movies    | https://api.themoviedb.org/3/movie/popular           |
| Get Movie             | https://api.themoviedb.org/3/movie/{id}              |
| Get Images            | https://image.tmdb.org/t/p/{image-size}/{image-path} |
| MovieDB Documentation | https://developers.themoviedb.org/3/getting-started  |
**2. Display movies inside a Lane component**
The fetched assets will be rendered inside the `HeroLane` component with its background image, title, description, genres and the length (see design). The design uses the font Arial and Arial Black.
Asset Properties:
- Background Image: `backdrop_path`
- Genres: `genres`
- Title: `title`
- Description: `overview`
- Length: `runtime`
![Hero Lane](hero-lane.png)
_OPTIONAL_: You do NOT need to implement the carousel behaviour for the component, however you can if you like. The arrows in the design on the left and right behave like a carousel and will show the next card in the centered position after clicking. There is no animation needed at the moment.
**3. Implement text truncate for description**
Older SmartTVs use browsers that do not support some of the newer CSS features like _line-clamp_. As we need to support also those devices in the future, we would ask you to implement the `truncate()` function for the text description. The text should render three dots at the end `(...)` and should not cut in the middle of words. We do not require at what point the whole text should be truncated, however we would like configure it. For example the text might be truncated at 50% per default but can be modified as well.
Write suitable unit tests for this function. Additionally think about performance and prepare to discuss your thoughts about drawbacks and benefits of your solution.
### Tips
- Verify and fetch the correct image size
- We are not looking into pixel perfect implementation
- Using a different font is completely fine
- We recommend usage of types
- No need to support browsers that you do not like
- Use any CSS library of your choice
- Think about the sad path (error handling)
- Unit tests are your friends
### Emergency contact
Please ask any question if something is not understandable.
Tkachuk Artem: [arte.tkachuk@gmail.com](arte.tkachuk@gmail.com)
> Happy coding and may the duck be with you!
