#   S K G - I F   S H A C L   E x t r a c t o r  
  
 A   P y t h o n   t o o l   t o   a u t o m a t i c a l l y   g e n e r a t e   S H A C L   s h a p e s   f r o m   O W L   o n t o l o g i e s   t h a t   f o l l o w   t h e   S K G - I F   d o c u m e n t a t i o n   p a t t e r n .  
  
 # #   D e s c r i p t i o n  
  
 T h i s   t o o l   e x t r a c t s   S H A C L   ( S h a p e s   C o n s t r a i n t   L a n g u a g e )   s h a p e s   f r o m   O W L   o n t o l o g i e s   t h a t   u s e   a   s p e c i f i c   d o c u m e n t a t i o n   p a t t e r n   f o r   d e s c r i b i n g   c l a s s   p r o p e r t i e s .   I t   p a r s e s   p r o p e r t y   d e s c r i p t i o n s   i n   t h e   f o r m a t :  
  
 -   p r o p e r t y N a m e   - [ c a r d i n a l i t y ] - >   t a r g e t T y p e  
  
 F o r   e x a m p l e :  
  
 -   d c t e r m s : t i t l e   - [ 1 ] - >   r d f s : L i t e r a l  
 -   f r a p o : h a s G r a n t N u m b e r   - [ 0 . . 1 ] - >   x s d : s t r i n g  
 -   f r a p o : h a s F u n d i n g A g e n c y   - [ 0 . . 1 ] - >   f r a p o : F u n d i n g A g e n c y  
  
 # #   R e q u i r e m e n t s  
  
 -   P y t h o n   3 . 9 +  
 -   P o e t r y   f o r   d e p e n d e n c y   m a n a g e m e n t  
  
 # #   I n s t a l l a t i o n  
  
 1 .   C l o n e   t h e   r e p o s i t o r y  
 2 .   I n s t a l l   d e p e n d e n c i e s   u s i n g   [ P o e t r y ] ( h t t p s : / / p y t h o n - p o e t r y . o r g / ) :  
  
 ` ` ` b a s h  
 p o e t r y   i n s t a l l  
 ` ` `  
  
 # #   U s a g e  
  
 T o   r u n   t h e   t o o l ,   u s e   t h e   f o l l o w i n g   c o m m a n d :  
  
 ` ` ` b a s h  
 p o e t r y   r u n   s r c . m a i n   < i n p u t _ f i l e >   < o u t p u t _ f i l e >  
 ` ` `  
  
 O r   i f   y o u   w a n t   t o   r u n   i t   d i r e c t l y :  
  
 ` ` ` b a s h  
 p y t h o n   - m   s r c . m a i n   < i n p u t _ f i l e >   < o u t p u t _ f i l e >  
 ` ` `  
  
 w h e r e :  
 -   ` i n p u t _ f i l e ` :   P a t h   t o   t h e   i n p u t   O W L   o n t o l o g y   f i l e   i n   T u r t l e   ( . t t l )   f o r m a t .   T h i s   f i l e   s h o u l d   c o n t a i n   c l a s s   d e f i n i t i o n s   w i t h   p r o p e r t y   d e s c r i p t i o n s   f o l l o w i n g   t h e   S K G - I F   d o c u m e n t a t i o n   p a t t e r n .  
 -   ` o u t p u t _ f i l e ` :   P a t h   w h e r e   t h e   g e n e r a t e d   S H A C L   s h a p e s   w i l l   b e   s a v e d   ( i n   T u r t l e   f o r m a t ) .   T h e   t o o l   w i l l   c r e a t e   o r   o v e r w r i t e   t h i s   f i l e .  
  
 E x a m p l e :  
 ` ` ` b a s h  
 p y t h o n   - m   m a i n   o n t o l o g y . t t l   s h a p e s . t t l  
 ` ` `  
  
 # #   T e s t i n g  
  
 R u n   t h e   u n i t   t e s t s :  
  
 ` ` ` b a s h  
 p y t h o n   - m   u n i t t e s t  
 ` ` `  
  
 # #   L i c e n s e  
  
 I S C   L i c e n s e  
  
 # #   A u t h o r  
  
 A r c a n g e l o   M a s s a r i   ( a r c a n g e l o . m a s s a r i @ u n i b o . i t ) 