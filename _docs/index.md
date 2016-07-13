---
layout: page
title:  "Docs"
page-class: c-page--docs
has-sub-content: true
sub-content: docs
permalink: /docs/
---
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus, voluptatum reiciendis provident dignissimos repudiandae qui ratione nam dicta officia, quidem illo non id laboriosam, eum recusandae assumenda repellat autem. Suscipit.

<h3>Lorem ipsum dolor sit.</h3>

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsam ducimus sunt nemo ex, deleniti, minus facilis fugiat distinctio cupiditate minima atque obcaecati reprehenderit quis rem. Facilis, illum hic. Quas, laborum.

<ul>
  {% for page in site.pages %}
    {% if page.categories == 'docs' and page.tags == 'general' %}
      <li>
        <a href="{{ page.url }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

<ul>
  <li>
    <a href="/docs/settings/settings.html">Settings</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'settings' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/tools/tools.html">Tools</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'tools' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/generic/generic.html">Generic</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'generic' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/elements/elements.html">Elements</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'elements' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/objects/objects.html">Objects</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'objects' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/components/components.html">Components</a>
  </li>
</ul>

<ul>
  <li>
    <a href="/docs/utilities/utilities.html">Utilities</a>
    <ul>
      {% for page in site.pages %}
        {% if page.categories == 'docs' and page.tags == 'utilities' %}
          <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>


Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro fugit fuga, laboriosam, atque, corporis alias ratione id quos est omnis assumenda ipsa cumque animi. Explicabo quos voluptas, expedita deleniti sapiente culpa nulla tempora exercitationem suscipit. Tempora fuga odit laudantium sit dolores magnam officiis rerum autem quidem assumenda officia beatae et, delectus consectetur repellat aspernatur quae inventore vero adipisci veniam, iure sapiente eligendi harum temporibus. Perferendis, ratione, assumenda! Odit est, laudantium? Quibusdam dicta voluptate perferendis adipisci fuga enim magnam, ducimus optio voluptatibus natus amet libero illo, reprehenderit distinctio cum fugit illum, accusantium excepturi sit soluta eum. Commodi debitis quod numquam?

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsa voluptatem aperiam impedit libero natus quas quibusdam voluptatum inventore at incidunt commodi id rem dicta enim deserunt vel nam porro amet corrupti perspiciatis magni, vitae molestias quidem consequatur! Facere eligendi explicabo, harum blanditiis deserunt hic a magni fuga at adipisci excepturi, provident necessitatibus. Hic harum enim, minima architecto fuga, accusantium quibusdam asperiores. Eligendi vero ducimus suscipit asperiores error, quam quibusdam! Dolorem modi atque consectetur earum eum vero.

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Numquam excepturi maxime deserunt beatae aliquam, commodi exercitationem illo? Nemo, eveniet eaque corporis magni temporibus expedita consectetur facere, nesciunt esse porro ab repellat ducimus amet pariatur, nihil consequatur cum eius. Maxime praesentium optio cumque perferendis, provident porro laudantium modi, eius ad asperiores, excepturi adipisci. Voluptates inventore provident doloribus, consequatur fugiat, molestiae explicabo dolore ea dolor blanditiis aliquid ducimus eum eius, obcaecati magni incidunt cum doloremque in deleniti maxime distinctio? Enim, obcaecati quisquam adipisci consequatur excepturi eos impedit consequuntur mollitia corporis, rerum, asperiores, maxime quos suscipit cupiditate laboriosam accusantium natus voluptatum est. Necessitatibus quo quidem aliquid eligendi enim, consequatur impedit illum nam culpa dignissimos facere dolorum repellendus neque praesentium aut ipsam et totam.
