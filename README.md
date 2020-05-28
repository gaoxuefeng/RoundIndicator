# RoundIndicator

**A package for TabBar to create round indicator **
**RoundIndicator是用来创建圆角indicator的一个库**

使用方法:
###  
              TabBar(
                isScrollable: true,
                controller: tabController,
                labelStyle: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
                unselectedLabelStyle: TextStyle(fontSize: 20, fontWeight: FontWeight.normal),
                labelColor: Colors.black,
                indicator: RoundTabIndicator(
                    borderSide: BorderSide(color: MyColors.fromARGBString("#da4da9"), width: 3),
                    gradient: LinearGradient(colors: [Colors.red, Colors.black]),
                    isRound: true,
                    radius: 2,
                    insets: EdgeInsets.only(left: 15, right: 15)),
                onTap: (index) {
                  tabIndex = index;
                  setState(() {});
                },
                tabs: tabs.map((tabName) {
                  return Tab(
                    child: Center(
                      child: Container(
                        child: Center(
                          child: Text(tabName),
                        ),
                      ),
                    ),
                  );
                }).toList(),
              ),
            ),
			  
![Image](https://github.com/gaoxuefeng/RoundIndicator/blob/master/image1.png?raw=true)


### End