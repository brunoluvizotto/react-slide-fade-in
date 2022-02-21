# React Slide Fade In

A container component that will add a slide fade in animation to children elements.

![slide-fade-in](https://user-images.githubusercontent.com/8275052/154869937-6a9d163b-e8b7-4db2-b729-24457d428ac8.gif)

## Installation

`yarn add react-slide-fade-in`

or

`npm install react-slide-fade-in`

## Props

The container component receives the following props:
```typescript
{
  // Position to slide in from
  from: 'top' | 'bottom' | 'left' | 'right' 

  // Offset from final position in pixels
  positionOffset: number

  // Offset for the trigger in pixels 
  // (to trigger before or after the final position is visible)
  triggerOffset: number

  // [Optional] Fade animation start delay in milliseconds. Default: 0 ms
  delayInMilliseconds?: number

  // [Optional] Fade animation duration in milliseconds. Default: 1200 ms
  durationInMilliseconds?: number
}
```

## Usage

```typescript
import { FadeIn } from 

export const Example: FC = () => (
  <div>
    <FadeIn 
      from="bottom"
      positionOffset={400}
      triggerOffset={200}
      delayInMilliseconds={0}
    >
      Child 1
    </FadeIn>
    <FadeIn
      from="top"
      positionOffset={400}
      triggerOffset={400}
      delayInMilliseconds={200}
    >
      Child 2
    </FadeIn>
    <FadeIn
      from="left"
      positionOffset={400}
      triggerOffset={200}
      delayInMilliseconds={400}
    >
      Child 3
    </FadeIn>
    <FadeIn
      from="right"
      positionOffset={400}
      triggerOffset={200}
      delayInMilliseconds={600}
    >
      Child 4
    </FadeIn>
    <FadeIn
      from="bottom"
      positionOffset={0}
      triggerOffset={0}
      delayInMilliseconds={800}
    >
      Child 5
    </FadeIn>
    <FadeIn
      from="bottom"
      positionOffset={0}
      triggerOffset={0}
      delayInMilliseconds={1000}
    >
      Child 6
    </FadeIn>
  </div>
)
```
