<style>
  .stylish {
    font-family: var(--slantText);
    font-size: var(--h3);
  }

  .stylish-small {
    font-family: var(--slantText);
    font-size: var(--smallTextSize);
  }

  .addSpace {
    margin-bottom: 5%;
  }

  .split {
    display: grid;
    grid-template-columns: 33% 67%;
    grid-gap: 20px;
  }
</style>

<h1>Test Classless Styles</h1>

<p>
  Lorem ipsum dolor sit amet,
  <a href="/about">consectetur</a>
  adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
  aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
  nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
  reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
  Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
  deserunt mollit anim id est laborum.
</p>

<h2>Test Classless Styles</h2>
<h3>Hello World</h3>
<h4>Hello World</h4>
<h5>Hello World</h5>
<h6>Hello World</h6>

<div class="split">
  <aside>
    <p>
      Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
      deserunt mollit anim id est laborum.
    </p>
  </aside>
  <p>
    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
    deserunt mollit anim id est laborum.
  </p>
</div>

<hr />

<p class="stylish-small">This text should be supper pretty</p>

<blockquote>
  Lorem ipsum dolor sit amet,
  <strong>consectetur</strong>
  adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
  aliqua. Ut enim ad minim veniam, quis nostrud exercitation
  <a href="/about">consectetur</a>
  ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
  in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
  pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
  officia deserunt mollit anim id est laborum.
</blockquote>
<hr />

<p class="stylish">This text should be supper pretty</p>
<div class="grid">

  <p>
    Lorem ipsum dolor sit amet,
    <a href="/about">consectetur</a>
    adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
    aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
    nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
    reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
    pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
    officia deserunt mollit anim id est laborum.
  </p>
  <ul>
    <li>item here</li>
    <li>another item here</li>
    <li>last item for now</li>
  </ul>
</div>

<div class="card addSpace">
  <h3>Card Heading</h3>
  <p>
    adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
    aliqua.
  </p>
  <button>Accept</button>
</div>

<hr />

<form class="grid cols-3">
  <div>
    <label for="text">Text</label>
    <input id="text" type="text" placeholder="Jon Palacio" />
  </div>
  <div>
    <label for="number">Number</label>
    <input id="number" type="number" />
  </div>
  <div>
    <label for="email">Email</label>
    <input id="email" type="email" />
  </div>
</form>
<div>
  <label for="textarea">Textarea</label>
  <textarea id="textarea">Default Value</textarea>
</div>
<div>
  <label for="select">Select</label>
  <select id="select" type="text">
    <option value="one">One</option>
    <option value="two">Two</option>
    <option value="three">Three</option>
  </select>
</div>

<button>Submit</button>
<button class="cancel">Cancel</button>
<button disabled>Disabled</button>
<button>Button with long text</button>
<button>Button &xrarr;</button>
<br />
<button class="small">Small</button>
