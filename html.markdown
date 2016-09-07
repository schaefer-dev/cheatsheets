# HTML Markdown

## Tags (x inside <> with closing /x in <>)

* Header
    * <h1> h1 for a huge header </h1>
    * <h2> h2 - a slightly smaller header. Still pretty big though. </h2>
    * <h3> h3 - finally getting a bit smaller. </h3>
    * <h4> h4: pretty usual font size with  </h4> <h5> and h5 </h5> 
    * <h6> till really small h6 </h6>

* p for paragraph
* ul for unordered list (with li as the bullet-points/ list elements)
* ol for odered list (as well with li as list elements this time with counting numbers in front

### Self-closing tags
    * <hr /> for a seperating rule
    * <br /> for a linebreak

### text-formatting tags
    * <strong> bold text </strong>
    * <em> italics </em>
    * <u> underlined text </u>
    * <strike> crossed out text </strike>

### Pictures
    * self closing tag <img x /> usually with source given like this <img src="source" />
    * source can be a filepath of the file uploaded inside public_html or a URL
    * further properties can be set after the source like this <img src="source" width="100" />
        * width for image width (scaled)
        * height for image height (again scaled)

### Forms
    * <form> Form </form>
    * input: (<input /> self closing)
        * type has to be set with type="x" ex. text, email
        * optional: set prevalue with value="x"
        * optional: set placeholder with placeholder="x"
    * <textarea> textarea </textarea>
    * selectwindow (<select> </select>)
        * with various options set with <option> Option </option>
    * <input type="radio" /> x - for to tick circle x
        * categorize circles together so that only one of them can be selected at a time <input type="radio" name="x" /> so all further circles with name x will be bond together
    * <input type="checkbox" /> x - for selectable box 
    * <input type="submit" /> for submit button
    * name="x" can be added to all of those inputs so that submit saves the value under the given name (in case of checkboxes possible to also set a value for ex. 1 in case it is ticked)

### Links
    * <a href="http://www.google.com" > Google as an example </a> (href for hyperlink reference (external link) or other html file on your server (internal link))
    * link for movement on the very same page with at the position we want to be able to go to <a name="x" /> and <a href="#x"> linktext here </a> for the actual link.

### Tables
    * consists of tablerows (tr) and tablecells (td) with tableheaders (th)
    * example: 
        <table>
             <tr> <th>name</th> <th>age</th> <th>gender</th> </tr>
             <tr> <td>Daniel</td> <td>20</td> <td>m</td> </tr>
             <tr> <td>Jonas</td> <td>15</td> <td>m</td> </tr>
             <tr> <td>Stefan</td> <td>52</td> <td>m</td> </tr>
             <tr> <td>Annette</td> <td>51</td> <td>f</td> </tr>
        </table>

### Entities
    * used for symbols like < with &lt; and so on
    * for reference look up on http://www.w3schools.com/html/html_entities.asp

### iFrame
    * similiar to links use <iframe src="x"> </iframe> to show the content of a website or of a local server html-file inside the webpage (works also with yt videos see embedded!)
    * youtube example: <iframe width="560" height="315" src="https://www.youtube.com/embed/LgFFO32Tdlo" frameborder="0" allowfullscreen></iframe>

###
