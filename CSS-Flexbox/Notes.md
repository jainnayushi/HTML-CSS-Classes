1. basic styles
2. display flex to box-wrapper
display:flex;
3. terminologies

># Flex Container : index.css

4. flex-direction : main-axis
 flex-direction: row; 
 flex-direction: row-reverse; 
 flex-direction: column; 
 flex-direction: column-reverse; 

5. flex-wrap : cross-axis
flex-wrap : wrap
flex-wrap : nowrap
flex-wrap : wrap-reverse
 
* Play 
height:400px
flex-direction: column
flex-wrap :wrap

6. justify-content : main-axis
  /* justify-content: flex-start; */
  /* justify-content: flex-end; */
  /* justify-content: center; */
  /* justify-content: space-between; */
  /* justify-content: space-around; */
  /* justify-content: space-evenly; */

* Play 
height:900px
flex-direction: column
justify-content:center

7. align-items : cross-axis
  /* align-items: stretch; */
  /* align-items: flex-start; */
  /* align-items: flex-end; */
  /* align-items: center; */

8. flex-flow : flex-direction flex-wrap
  /* flex-flow: row nowrap; */
  /* flex-flow: row wrap; */
  /* flex-flow: column wrap; */
  /* flex-flow: column nowrap; */

===

># Flex-Items : style.css

1. align-self : 
* overrides align align-item
  /* align-self: stretch; */
  /* align-self: flex-start; */
  /* align-self: flex-end; */
  /* align-self: center; */

2. order
* greater the order - afterwards it will be
order :0

3. flex-basis
* initial length towards main axis

4. flex-grow
* rate of occupying available space
 flex-grow: 1; - equally occupy left space of container
 flex-grow: 2; - twice the left space

5. flex-shrink
* 
 flex-shrink: 1; - equally give up the space of container
 flex-shrink: 2; - give up twice the  space

6. flex : flex-grow flex-shrink flex-basis
flex: 1 2 300px