This document includes personal answers/declarations of the most curious subjects and asked questions about iOS development.

- [Subjects](#subjects)
  - [Course Suggestion](#course-suggestion) 
  - [Building UI, Storyboard vs Programmatically](#building-ui-storyboard-vs-programmatically)
- [Questions](#questions)
  - [Which One Should I Start with, UIKit or SwiftUI?](#which-one-should-i-start-with-uikit-or-swiftui)

## Subjects

### Course Suggestion
Good course, good start. Hence, I suggest these,
- [Hacking with Swift](https://www.hackingwithswift.com/learn)
- [iOS & Swift Development from Angela Yu](https://www.udemy.com/course/ios-13-app-development-bootcamp/)

### Building UI, Storyboard vs Programmatically
Well, I know only a few people who like storyboards(some of them are already the developers who built storyboard). In case you are in the beginning of your iOS development career, you absolutely should start with Storybard to build UI. When the situation is visualized, human brain gets the situation easier. You should focus on [auto layout](https://developer.apple.com/library/archive/documentation/UserExperience/Conceptual/AutolayoutPG/index.html) first by getting help from visualizing.

I prefer building UI programmatically like most developers. Storyboard or XIB files are not useful in my opinion. When you open a storyboard and focus on a view that has a lot of subviews aligned vertically, just take one of them in the middle and move to the bottom. The view will look like some crazy stuff happened. Visualizing will not help you anymore. 

On the other hand in building UI programmatically, you only care about the anchors(constraint positions) of the views. You can easily change/switch anchors because they are in a class. I recommend using [SnapKit](https://github.com/SnapKit/SnapKit) to build UI programmatically. It provides a cool and clear syntax. You can also create your NSLayoutConstraint extensions.

## Questions

### Which One Should I Start with, UIKit or SwiftUI?
In 2022, most companies still use UIKit actively. In case you work for a company, you will most probably face with a project written in UIKit, not SwiftUI. Also, SwiftUI has still some weaknesses rather than UIKit. When you come over a weakness of SwiftUI, you must build a bridge via UIKit by using [UIViewRepresentable](https://developer.apple.com/documentation/swiftui/uiviewrepresentable). You must have UIKit knowledge to build that bridge.  

In conclusion, it is better to start with UIKit. After you have a job and you feel that you are okay with UIKit knowledge, you are free to improve our SwiftUI skills in your free time except during working hours.
