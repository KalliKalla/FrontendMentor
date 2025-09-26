Your Current Structure - The Good:

✅ Using <main> for primary content - excellent semantic choice!✅ BEM naming convention attempt with card\_\_ prefix✅ Proper viewport meta tag✅
Using heading tags (though we need to discuss hierarchy)

Critical Issues & Teaching Points:

1. Missing Profile Image

You've completely omitted Jessica's profile picture! This is the visual anchor of the design.

Teaching Point: Always identify ALL visual elements in a design before coding. I recommend creating a quick checklist from the design first.

2. Heading Hierarchy Problem

  <h1 class="card__name">Jessica Randall</h1>
  <h2 class="card__location">London, United Kingdom</h2>

Issue: "London, United Kingdom" is NOT a heading - it's descriptive text about Jessica. Using <h2> here breaks semantic meaning.

Better approach:

  <h1 class="card__name">Jessica Randall</h1>
  <p class="card__location">London, United Kingdom</p>

Teaching Point: Headings (h1-h6) represent document outline structure, not visual importance. Ask yourself: "Is this a section title?" If no,
it's not a heading.

3. Links Aren't Links!

  <div class="card__social-link">GitHub</div>

Major Issue: These should be clickable <a> tags, not <div> elements!

Why this matters:

- Accessibility: Screen readers won't announce these as interactive
- Keyboard navigation: Users can't tab to them
- SEO/Semantics: Search engines won't understand these are links
- User expectation: No hover cursor, no default link behaviors

Correct approach:
<a href="https://github.com/username" class="card__social-link">GitHub</a>

4. Missing Semantic Structure

Your links container could be more semantic. Consider:

  <nav class="card__social-links" aria-label="Social media links">
    <ul>
      <li><a href="#">GitHub</a></li>
      <li><a href="#">Frontend Mentor</a></li>
      <!-- etc -->
    </ul>
  </nav>

Why?

- <nav> tells assistive tech this is a navigation region
- Lists announce "5 items" to screen readers
- Better CSS flexibility without affecting semantics

5. Missing Role Context

The bio text lacks semantic context:

  <p>"Front-end developer and avid reader."</p>

Better:

  <p class="card__bio">"Front-end developer and avid reader."</p>

Recommended Complete Structure:

Here's how I'd approach it as a veteran developer:

  <main class="profile-card">
    <article class="card">
      <img src="./assets/images/avatar-jessica.jpeg"
           alt="Jessica Randall"
           class="card__avatar">

      <h1 class="card__name">Jessica Randall</h1>
      <p class="card__location">London, United Kingdom</p>
      <p class="card__bio">"Front-end developer and avid reader."</p>

      <nav class="card__links" aria-label="Social media profiles">
        <ul>
          <li>
            <a href="https://github.com" class="card__link">GitHub</a>
          </li>
          <!-- repeat for other links -->
        </ul>
      </nav>
    </article>

  </main>

Key Lessons:

1. Semantics First: Choose HTML elements for what they MEAN, not how they LOOK
2. Accessibility is NOT Optional: Every div that should be interactive needs proper semantic elements
3. Test Without CSS: Your HTML should make sense even with CSS disabled
4. Keyboard Navigation: Can you tab through everything interactive?

Questions for You:

1. Why do you think I wrapped the card in an <article> tag?
2. What would happen if a screen reader user encountered your current version?
3. How would you make the profile image a perfect circle using CSS?

Want me to explain any of these concepts in more depth?
