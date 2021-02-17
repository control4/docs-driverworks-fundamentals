## Proxy Binding Single Proxy Examples


```xml
<connection>
      <id>5001</id>
      <facing>6</facing>
      <connectionname>TV</connectionname>
      <type>2</type>
      <consumer>False</consumer>
      <audiosource>False</audiosource>
      <videosource>False</videosource>
      <linelevel>False</linelevel>
      <classes>
         <class>
            <classname>TV</classname>
         </class>
      </classes>
</connection>
```



```xml
<connection>
      <id>5001</id>
      <facing>6</facing>
      <connectionname>Light</connectionname>
      <type>2</type>
      <consumer>True</consumer>
      <audiosource>False</audiosource>
      <videosource>False</videosource>
      <linelevel>False</linelevel>
      <classes>
         <class>
            <classname>LIGHT</classname>
            <autobind>False</autobind>
         </class>
      </classes>
      <hidden>False</hidden>
</connection>
```
